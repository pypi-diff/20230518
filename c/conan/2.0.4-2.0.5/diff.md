# Comparing `tmp/conan-2.0.4.tar.gz` & `tmp/conan-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.0.4.tar", last modified: Tue Apr 11 14:41:59 2023, max compression
+gzip compressed data, was "dist/conan-2.0.5.tar", last modified: Thu May 18 13:49:06 2023, max compression
```

## Comparing `conan-2.0.4.tar` & `conan-2.0.5.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.097133 conan-2.0.4/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-04-11 14:41:51.000000 conan-2.0.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 14:41:51.000000 conan-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8324 2023-04-11 14:41:59.097133 conan-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6041 2023-04-11 14:41:51.000000 conan-2.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.052132 conan-2.0.4/conan/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.053132 conan-2.0.4/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     6824 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.056132 conan-2.0.4/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11124 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3144 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4425 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     3907 2023-04-11 14:41:51.000000 conan-2.0.4/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.057132 conan-2.0.4/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7473 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    11022 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     7512 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.061132 conan-2.0.4/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     4419 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8119 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    11692 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     3830 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.061132 conan-2.0.4/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.062132 conan-2.0.4/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5019 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.062132 conan-2.0.4/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4741 2023-04-11 14:41:51.000000 conan-2.0.4/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-11 14:41:51.000000 conan-2.0.4/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.063132 conan-2.0.4/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.065132 conan-2.0.4/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     7076 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12247 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.066132 conan-2.0.4/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10153 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     7931 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5264 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-04-11 14:41:51.000000 conan-2.0.4/conan/internal/integrity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.067133 conan-2.0.4/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.068132 conan-2.0.4/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11201 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16202 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.069133 conan-2.0.4/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11104 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    15410 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.070133 conan-2.0.4/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      269 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9956 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.070133 conan-2.0.4/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.071133 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3848 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    19484 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/file_api.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    14423 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.072133 conan-2.0.4/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35862 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    11205 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.073133 conan-2.0.4/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25269 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.074133 conan-2.0.4/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/cpp_package.py
--rw-r--r--   0 root         (0) root         (0)    24621 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     5824 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.074133 conan-2.0.4/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.075133 conan-2.0.4/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      274 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13040 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3557 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    17816 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    10956 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.076133 conan-2.0.4/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.077133 conan-2.0.4/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    22075 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.078133 conan-2.0.4/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    10844 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.078133 conan-2.0.4/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    11503 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9874 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8619 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.079133 conan-2.0.4/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16286 2023-04-11 14:41:51.000000 conan-2.0.4/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.053132 conan-2.0.4/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8324 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9035 2023-04-11 14:41:59.000000 conan-2.0.4/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      470 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 14:41:58.000000 conan-2.0.4/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.080133 conan-2.0.4/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2023-04-11 14:41:51.000000 conan-2.0.4/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.083133 conan-2.0.4/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.083133 conan-2.0.4/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9791 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/editable.py
--rw-r--r--   0 root         (0) root         (0)     6843 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cache/remote_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.084133 conan-2.0.4/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7619 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12827 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/uploader.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/cmd/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.085133 conan-2.0.4/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     6307 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9195 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)    14016 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9235 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6124 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.086133 conan-2.0.4/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)     8621 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.089133 conan-2.0.4/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    12000 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    16237 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    16785 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    11680 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     6536 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5726 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21352 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    16751 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    11423 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.090133 conan-2.0.4/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5987 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     5388 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)    10011 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.090133 conan-2.0.4/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-04-11 14:41:51.000000 conan-2.0.4/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-04-11 14:41:51.000000 conan-2.0.4/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-04-11 14:41:51.000000 conan-2.0.4/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7819 2023-04-11 14:41:51.000000 conan-2.0.4/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-04-11 14:41:51.000000 conan-2.0.4/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.093133 conan-2.0.4/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21687 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    11676 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    29539 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)     9578 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17065 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     7583 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    23711 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13231 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6038 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-04-11 14:41:51.000000 conan-2.0.4/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.093133 conan-2.0.4/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-11 14:41:51.000000 conan-2.0.4/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-04-11 14:41:51.000000 conan-2.0.4/conans/pylint_plugin.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 14:41:51.000000 conan-2.0.4/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.094133 conan-2.0.4/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4384 2023-04-11 14:41:51.000000 conan-2.0.4/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.094133 conan-2.0.4/conans/test/
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13174 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.095133 conan-2.0.4/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    34736 2023-04-11 14:41:51.000000 conan-2.0.4/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:41:59.096134 conan-2.0.4/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-04-11 14:41:51.000000 conan-2.0.4/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-11 14:41:59.097133 conan-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5058 2023-04-11 14:41:51.000000 conan-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.151381 conan-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-05-18 13:48:59.000000 conan-2.0.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 13:48:59.000000 conan-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-05-18 13:49:06.152381 conan-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-05-18 13:48:59.000000 conan-2.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.107377 conan-2.0.5/conan/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.108377 conan-2.0.5/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.111378 conan-2.0.5/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4478 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.111378 conan-2.0.5/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.115378 conan-2.0.5/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8474 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     8632 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.115378 conan-2.0.5/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.116378 conan-2.0.5/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.116378 conan-2.0.5/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5649 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-18 13:48:59.000000 conan-2.0.5/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.119378 conan-2.0.5/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.120378 conan-2.0.5/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.120378 conan-2.0.5/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/integrity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.121379 conan-2.0.5/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.121379 conan-2.0.5/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.122379 conan-2.0.5/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11201 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16380 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.123379 conan-2.0.5/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    15410 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.124379 conan-2.0.5/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9956 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.124379 conan-2.0.5/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.125379 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5704 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    19484 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/file_api.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    14423 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.126379 conan-2.0.5/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35919 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.126379 conan-2.0.5/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25389 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.127379 conan-2.0.5/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/cpp_package.py
+-rw-r--r--   0 root         (0) root         (0)    24621 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     5824 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.128379 conan-2.0.5/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.129379 conan-2.0.5/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13228 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    10956 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.131379 conan-2.0.5/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    22075 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.132379 conan-2.0.5/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10592 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9874 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8619 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.134380 conan-2.0.5/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16286 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.108377 conan-2.0.5/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9035 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.135380 conan-2.0.5/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-18 13:48:59.000000 conan-2.0.5/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.137380 conan-2.0.5/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.138380 conan-2.0.5/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10687 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/editable.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/remote_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.138380 conan-2.0.5/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7671 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12827 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.139380 conan-2.0.5/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.140380 conan-2.0.5/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9195 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)    14006 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.140380 conan-2.0.5/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9459 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6126 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.141380 conan-2.0.5/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)     9520 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.143380 conan-2.0.5/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    14526 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    16759 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    15815 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    16848 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    11423 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.144380 conan-2.0.5/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     5388 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    10011 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    13590 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.144380 conan-2.0.5/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-18 13:48:59.000000 conan-2.0.5/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-18 13:48:59.000000 conan-2.0.5/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7817 2023-05-18 13:48:59.000000 conan-2.0.5/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-18 13:48:59.000000 conan-2.0.5/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.147381 conan-2.0.5/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19581 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12460 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29433 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    10886 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24590 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6038 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.147381 conan-2.0.5/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-18 13:48:59.000000 conan-2.0.5/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-18 13:48:59.000000 conan-2.0.5/conans/pylint_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.148381 conan-2.0.5/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.148381 conan-2.0.5/conans/test/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.150381 conan-2.0.5/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    35320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.151381 conan-2.0.5/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11263 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-18 13:49:06.152381 conan-2.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5058 2023-05-18 13:48:59.000000 conan-2.0.5/setup.py
```

### Comparing `conan-2.0.4/LICENSE.md` & `conan-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/PKG-INFO` & `conan-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.4
+Version: 2.0.5
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.4/README.md` & `conan-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/conan_api.py` & `conan-2.0.5/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/model.py` & `conan-2.0.5/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/output.py` & `conan-2.0.5/conan/api/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-import json
 import sys
 
 from colorama import Fore, Style
 
 from conans.client.userio import color_enabled
+from conans.errors import ConanException
 from conans.util.env import get_env
 
 LEVEL_QUIET = 80  # -q
-
 LEVEL_ERROR = 70  # Errors
 LEVEL_WARNING = 60  # Warnings
 LEVEL_NOTICE = 50  # Important messages to attract user attention.
 LEVEL_STATUS = 40  # Default - The main interesting messages that users might be interested in.
 LEVEL_VERBOSE = 30  # -v  Detailed informational messages.
 LEVEL_DEBUG = 20  # -vv Closely related to internal implementation details
 LEVEL_TRACE = 10  # -vvv Fine-grained messages with very low-level implementation details
 
 
-# Singletons
-conan_output_level = LEVEL_STATUS
-
-
-def log_level_allowed(level):
-    return conan_output_level <= level
-
-
 class Color(object):
     """ Wrapper around colorama colors that are undefined in importing
     """
     RED = Fore.RED  # @UndefinedVariable
     WHITE = Fore.WHITE  # @UndefinedVariable
     CYAN = Fore.CYAN  # @UndefinedVariable
     GREEN = Fore.GREEN  # @UndefinedVariable
@@ -53,21 +44,59 @@
     Color.BRIGHT_WHITE = Fore.BLACK
     Color.BRIGHT_CYAN = Fore.BLUE
     Color.BRIGHT_YELLOW = Fore.MAGENTA
     Color.BRIGHT_GREEN = Fore.GREEN
 
 
 class ConanOutput:
+    # Singleton
+    _conan_output_level = LEVEL_STATUS
+    _silent_warn_tags = []
+
     def __init__(self, scope=""):
         self.stream = sys.stderr
         self._scope = scope
         # FIXME:  This is needed because in testing we are redirecting the sys.stderr to a buffer
         #         stream to capture it, so colorama is not there to strip the color bytes
         self._color = color_enabled(self.stream)
 
+    @classmethod
+    def define_silence_warnings(cls, warnings):
+        cls._silent_warn_tags = warnings or []
+
+    @classmethod
+    def define_log_level(cls, v):
+        """
+        Translates the verbosity level entered by a Conan command. If it's `None` (-v),
+        it will be defaulted to `verbose` level.
+
+        :param v: `str` or `None`, where `None` is the same as `verbose`.
+        """
+        try:
+            level = {"quiet": LEVEL_QUIET,  # -vquiet 80
+                     "error": LEVEL_ERROR,  # -verror 70
+                     "warning": LEVEL_WARNING,  # -vwaring 60
+                     "notice": LEVEL_NOTICE,  # -vnotice 50
+                     "status": LEVEL_STATUS,  # -vstatus 40
+                     None: LEVEL_VERBOSE,  # -v 30
+                     "verbose": LEVEL_VERBOSE,  # -vverbose 30
+                     "debug": LEVEL_DEBUG,  # -vdebug 20
+                     "v": LEVEL_DEBUG,  # -vv 20
+                     "trace": LEVEL_TRACE,  # -vtrace 10
+                     "vv": LEVEL_TRACE  # -vvv 10
+                     }[v]
+        except KeyError:
+            raise ConanException(f"Invalid argument '-v{v}'")
+        else:
+            cls._conan_output_level = level
+
+    @classmethod
+    def level_allowed(cls, level):
+        return cls._conan_output_level <= level
+
     @property
     def color(self):
         return self._color
 
     @property
     def scope(self):
         return self._scope
@@ -80,46 +109,37 @@
     def is_terminal(self):
         return hasattr(self.stream, "isatty") and self.stream.isatty()
 
     def writeln(self, data, fg=None, bg=None):
         return self.write(data, fg, bg, newline=True)
 
     def write(self, data, fg=None, bg=None, newline=False):
-        if conan_output_level > LEVEL_NOTICE:
+        if self._conan_output_level > LEVEL_NOTICE:
             return self
         if self._color and (fg or bg):
             data = "%s%s%s%s" % (fg or '', bg or '', data, Style.RESET_ALL)
 
         if newline:
             data = "%s\n" % data
         self.stream.write(data)
         self.stream.flush()
         return self
 
     def rewrite_line(self, line):
         tmp_color = self._color
         self._color = False
-        TOTAL_SIZE = 70
-        LIMIT_SIZE = TOTAL_SIZE // 2 - 3
-        if len(line) > TOTAL_SIZE:
-            line = line[0:LIMIT_SIZE] + " ... " + line[-LIMIT_SIZE:]
-        self.write("\r%s%s" % (line, " " * (TOTAL_SIZE - len(line))))
+        total_size = 70
+        limit_size = total_size // 2 - 3
+        if len(line) > total_size:
+            line = line[0:limit_size] + " ... " + line[-limit_size:]
+        self.write("\r%s%s" % (line, " " * (total_size - len(line))))
         self.stream.flush()
         self._color = tmp_color
 
-    def _write_message(self, msg, level_str, fg=None, bg=None):
-        if conan_output_level == LEVEL_QUIET:
-            return
-
-        def json_encoder(_obj):
-            try:
-                return json.dumps(_obj)
-            except TypeError:
-                return repr(_obj)
-
+    def _write_message(self, msg, fg=None, bg=None):
         if isinstance(msg, dict):
             # For traces we can receive a dict already, we try to transform then into more natural
             # text
             msg = ", ".join([f"{k}: {v}" for k, v in msg.items()])
             msg = "=> {}".format(msg)
             # msg = json.dumps(msg, sort_keys=True, default=json_encoder)
 
@@ -134,66 +154,69 @@
             ret += "{}{}{}{}".format(fg or '', bg or '', msg, Style.RESET_ALL)
         else:
             ret += "{}".format(msg)
 
         self.stream.write("{}\n".format(ret))
 
     def trace(self, msg):
-        if log_level_allowed(LEVEL_TRACE):
-            self._write_message(msg, "TRACE", fg=Color.BRIGHT_WHITE)
+        if self._conan_output_level <= LEVEL_TRACE:
+            self._write_message(msg, fg=Color.BRIGHT_WHITE)
         return self
 
     def debug(self, msg):
-        if log_level_allowed(LEVEL_DEBUG):
-            self._write_message(msg, "DEBUG")
+        if self._conan_output_level <= LEVEL_DEBUG:
+            self._write_message(msg)
         return self
 
     def verbose(self, msg, fg=None, bg=None):
-        if log_level_allowed(LEVEL_VERBOSE):
-            self._write_message(msg, "VERBOSE", fg=fg, bg=bg)
+        if self._conan_output_level <= LEVEL_VERBOSE:
+            self._write_message(msg, fg=fg, bg=bg)
         return self
 
     def status(self, msg, fg=None, bg=None):
-        if log_level_allowed(LEVEL_STATUS):
-            self._write_message(msg, "STATUS", fg=fg, bg=bg)
+        if self._conan_output_level <= LEVEL_STATUS:
+            self._write_message(msg, fg=fg, bg=bg)
         return self
 
     # Remove in a later refactor of all the output.info calls
     info = status
 
     def title(self, msg):
-        if log_level_allowed(LEVEL_NOTICE):
-            self._write_message("\n======== {} ========".format(msg), "NOTICE",
+        if self._conan_output_level <= LEVEL_NOTICE:
+            self._write_message("\n======== {} ========".format(msg),
                                 fg=Color.BRIGHT_MAGENTA)
         return self
 
     def subtitle(self, msg):
-        if log_level_allowed(LEVEL_NOTICE):
-            self._write_message("\n-------- {} --------".format(msg), "NOTICE",
+        if self._conan_output_level <= LEVEL_NOTICE:
+            self._write_message("\n-------- {} --------".format(msg),
                                 fg=Color.BRIGHT_MAGENTA)
         return self
 
     def highlight(self, msg):
-        if log_level_allowed(LEVEL_NOTICE):
-            self._write_message(msg, "NOTICE", fg=Color.BRIGHT_MAGENTA)
+        if self._conan_output_level <= LEVEL_NOTICE:
+            self._write_message(msg, fg=Color.BRIGHT_MAGENTA)
         return self
 
     def success(self, msg):
-        if log_level_allowed(LEVEL_NOTICE):
-            self._write_message(msg, "NOTICE", fg=Color.BRIGHT_GREEN)
+        if self._conan_output_level <= LEVEL_NOTICE:
+            self._write_message(msg, fg=Color.BRIGHT_GREEN)
         return self
 
-    def warning(self, msg):
-        if log_level_allowed(LEVEL_WARNING):
-            self._write_message("WARN: {}".format(msg), "WARN", Color.YELLOW)
+    def warning(self, msg, warn_tag=None):
+        if self._conan_output_level <= LEVEL_WARNING:
+            if warn_tag is not None and warn_tag in self._silent_warn_tags:
+                return self
+            warn_tag_msg = "" if warn_tag is None else f"{warn_tag}: "
+            self._write_message(f"WARN: {warn_tag_msg}{msg}", Color.YELLOW)
         return self
 
     def error(self, msg):
-        if log_level_allowed(LEVEL_ERROR):
-            self._write_message("ERROR: {}".format(msg), "ERROR", Color.RED)
+        if self._conan_output_level <= LEVEL_ERROR:
+            self._write_message("ERROR: {}".format(msg), Color.RED)
         return self
 
     def flush(self):
         self.stream.flush()
 
 
 def cli_out_write(data, fg=None, bg=None, endline="\n", indentation=0):
```

### Comparing `conan-2.0.4/conan/api/subapi/cache.py` & `conan-2.0.5/conan/api/subapi/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import shutil
+import os
 
 from conan.internal.conan_app import ConanApp
 from conan.internal.integrity_check import IntegrityChecker
 from conans.errors import ConanException
 from conans.model.package_ref import PkgReference
 from conans.model.recipe_ref import RecipeReference
 from conans.util.files import rmdir
@@ -60,14 +60,24 @@
         :param temp: boolean, remove the temporary folders
         :return:
         """
 
         app = ConanApp(self.conan_api.cache_folder)
         if temp:
             rmdir(app.cache.temp_folder)
+            # Clean those build folders that didn't succeed to create a package and wont be in DB
+            builds_folder = app.cache.builds_folder
+            if os.path.isdir(builds_folder):
+                for subdir in os.listdir(builds_folder):
+                    folder = os.path.join(builds_folder, subdir)
+                    manifest = os.path.join(folder, "p", "conanmanifest.txt")
+                    info = os.path.join(folder, "p", "conaninfo.txt")
+                    if not os.path.exists(manifest) or not os.path.exists(info):
+                        rmdir(folder)
+
         for ref, ref_bundle in package_list.refs():
             ref_layout = app.cache.ref_layout(ref)
             if source:
                 rmdir(ref_layout.source())
             if download:
                 rmdir(ref_layout.download_export())
             for pref, _ in package_list.prefs(ref, ref_bundle):
```

### Comparing `conan-2.0.4/conan/api/subapi/config.py` & `conan-2.0.5/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/download.py` & `conan-2.0.5/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/export.py` & `conan-2.0.5/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/graph.py` & `conan-2.0.5/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/install.py` & `conan-2.0.5/conan/api/subapi/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,8 @@
         if deploy:
             base_folder = conanfile.folders.base_build
             mkdir(base_folder)
             do_deploys(self.conan_api, deps_graph, deploy, base_folder)
 
         conanfile.generators = list(set(conanfile.generators).union(generators or []))
         app = ConanApp(self.conan_api.cache_folder)
-        write_generators(conanfile, app.hook_manager)
+        write_generators(conanfile, app)
```

### Comparing `conan-2.0.4/conan/api/subapi/list.py` & `conan-2.0.5/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/local.py` & `conan-2.0.5/conan/api/subapi/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,7 +99,14 @@
     @staticmethod
     def test(conanfile):
         """ calls the 'test()' method of the current (user folder) test_package/conanfile.py
         """
         with conanfile_exception_formatter(conanfile, "test"):
             with chdir(conanfile.build_folder):
                 conanfile.test()
+
+    def inspect(self, conanfile_path, remotes, lockfile):
+        app = ConanApp(self._conan_api.cache_folder)
+        conanfile = app.loader.load_named(conanfile_path, name=None, version=None,
+                                          user=None, channel=None, remotes=remotes, graph_lock=lockfile)
+        return conanfile
+
```

### Comparing `conan-2.0.4/conan/api/subapi/lockfile.py` & `conan-2.0.5/conan/api/subapi/lockfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 import os
 
 from conan.api.output import ConanOutput
 from conan.cli import make_abs_path
+from conans.client.graph.graph import Overrides
 from conans.errors import ConanException
 from conans.model.graph_lock import Lockfile, LOCKFILE
 
 
 class LockfileAPI:
 
     def __init__(self, conan_api):
         self.conan_api = conan_api
 
     @staticmethod
-    def get_lockfile(lockfile=None, conanfile_path=None, cwd=None, partial=False):
+    def get_lockfile(lockfile=None, conanfile_path=None, cwd=None, partial=False, overrides=None):
         """ obtain a lockfile, following this logic:
         - If lockfile is explicitly defined, it would be either absolute or relative to cwd and
           the lockfile file must exist. If lockfile="" (empty string) the default "conan.lock"
           lockfile will not be automatically used even if it is present.
         - If lockfile is not defined, it will still look for a default conan.lock:
            - if conanfile_path is defined, it will be besides it
            - if conanfile_path is not defined, the default conan.lock should be in cwd
            - if the default conan.lock cannot be found, it is not an error
 
         :param partial: If the obtained lockfile will allow partial resolving
         :param cwd: the current working dir, if None, os.getcwd() will be used
         :param conanfile_path: The full path to the conanfile, if existing
         :param lockfile: the name of the lockfile file
+        :param overrides: Dictionary of overrides {overriden: [new_ref1, new_ref2]}
         """
         if lockfile == "":
             # Allow a way with ``--lockfile=""`` to optout automatic usage of conan.lock
             return
 
         cwd = cwd or os.getcwd()
         if lockfile is None:  # Look for a default "conan.lock"
             # if path is defined, take it as reference
             base_path = os.path.dirname(conanfile_path) if conanfile_path else cwd
             lockfile_path = make_abs_path(LOCKFILE, base_path)
             if not os.path.isfile(lockfile_path):
+                if overrides:
+                    raise ConanException("Cannot define overrides without a lockfile")
                 return
         else:  # explicit lockfile given
             lockfile_path = make_abs_path(lockfile, cwd)
             if not os.path.isfile(lockfile_path):
                 raise ConanException("Lockfile doesn't exist: {}".format(lockfile_path))
 
         graph_lock = Lockfile.load(lockfile_path)
         graph_lock.partial = partial
+
+        if overrides:
+            graph_lock._overrides = Overrides.deserialize(overrides)
         ConanOutput().info("Using lockfile: '{}'".format(lockfile_path))
         return graph_lock
 
     def update_lockfile_export(self, lockfile, conanfile, ref, is_build_require=False):
         # The package_type is not fully processed at export
         is_python_require = conanfile.package_type == "python-require"
         is_require = not is_python_require and not is_build_require
```

### Comparing `conan-2.0.4/conan/api/subapi/new.py` & `conan-2.0.5/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/profiles.py` & `conan-2.0.5/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/remotes.py` & `conan-2.0.5/conan/api/subapi/remotes.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,50 +44,47 @@
             remotes = filtered_remotes
         return remotes
 
     def disable(self, pattern):
         remotes = self.list(pattern, only_enabled=False)
         for r in remotes:
             r.disabled = True
-            self.update(r)
+            self.update(r.name, disabled=True)
         return remotes
 
     def enable(self, pattern):
         remotes = self.list(pattern, only_enabled=False)
         for r in remotes:
             r.disabled = False
-            self.update(r)
+            self.update(r.name, disabled=False)
         return remotes
 
     def get(self, remote_name):
         app = ConanApp(self.conan_api.cache_folder)
         return app.cache.remotes_registry.read(remote_name)
 
-    def add(self, remote: Remote, force=False):
+    def add(self, remote: Remote, force=False, index=None):
         app = ConanApp(self.conan_api.cache_folder)
-        app.cache.remotes_registry.add(remote, force=force)
+        app.cache.remotes_registry.add(remote, force=force, index=index)
 
-    def remove(self, remote_name):
+    def remove(self, pattern: str):
         app = ConanApp(self.conan_api.cache_folder)
-        remotes = self.list(remote_name, only_enabled=False)
+        remotes = self.list(pattern, only_enabled=False)
         for remote in remotes:
             app.cache.remotes_registry.remove(remote.name)
             users_clean(app.cache.localdb, remote.url)
 
-    def update(self, remote: Remote):
-        app = ConanApp(self.conan_api.cache_folder)
-        app.cache.remotes_registry.update(remote)
-
-    def move(self, remote: Remote, index: int):
+    def update(self, remote_name, url=None, secure=None, disabled=None, index=None):
         app = ConanApp(self.conan_api.cache_folder)
-        app.cache.remotes_registry.move(remote, index)
+        app.cache.remotes_registry.update(remote_name, url, secure, disabled=disabled,
+                                          index=index)
 
-    def rename(self, remote: Remote, new_name: str):
+    def rename(self, remote_name: str, new_name: str):
         app = ConanApp(self.conan_api.cache_folder)
-        app.cache.remotes_registry.rename(remote, new_name)
+        app.cache.remotes_registry.rename(remote_name, new_name)
 
     def user_info(self, remote: Remote):
         app = ConanApp(self.conan_api.cache_folder)
         return users_list(app.cache.localdb, remotes=[remote])[0]
 
     def login(self, remote: Remote, username, password):
         app = ConanApp(self.conan_api.cache_folder)
```

### Comparing `conan-2.0.4/conan/api/subapi/remove.py` & `conan-2.0.5/conan/api/subapi/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,16 @@
         else:
             # Remove all the prefs with all the prevs
             self._remove_all_local_packages(app, ref)
 
     @staticmethod
     def _remove_all_local_packages(app, ref):
         # Get all the prefs and all the prevs
-        pkg_ids = app.cache.get_package_references(ref)
-        all_package_revisions = []
-        for pkg_id in pkg_ids:
-            all_package_revisions.extend(app.cache.get_package_revisions_references(pkg_id))
-        for pref in all_package_revisions:
+        pkg_ids = app.cache.get_package_references(ref, only_latest_prev=False)
+        for pref in pkg_ids:
             package_layout = app.cache.pkg_layout(pref)
             app.cache.remove_package_layout(package_layout)
 
     def package(self, pref: PkgReference, remote: Remote):
         assert pref.ref.revision, "Recipe revision cannot be None to remove a package"
         assert pref.revision, "Package revision cannot be None to remove a package"
```

### Comparing `conan-2.0.4/conan/api/subapi/search.py` & `conan-2.0.5/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/api/subapi/upload.py` & `conan-2.0.5/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/args.py` & `conan-2.0.5/conan/cli/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
                         help="Do not raise an error if some dependency is not found in lockfile")
     parser.add_argument("--lockfile-out", action=OnceArgument,
                         help="Filename of the updated lockfile")
     parser.add_argument("--lockfile-packages", action="store_true",
                         help="Lock package-id and package-revision information")
     parser.add_argument("--lockfile-clean", action="store_true",
                         help="Remove unused entries from the lockfile")
+    parser.add_argument("--lockfile-overrides",
+                        help="Overwrite lockfile overrides")
 
 
 def add_common_install_arguments(parser):
     parser.add_argument("-b", "--build", action="append", help=_help_build_policies)
 
     group = parser.add_mutually_exclusive_group()
     group.add_argument("-r", "--remote", action="append", default=None,
```

### Comparing `conan-2.0.4/conan/cli/cli.py` & `conan-2.0.5/conan/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,15 @@
             self._print_similar(command_argument)
             raise ConanException("Unknown command %s" % str(exc))
 
         try:
             command.run(self._conan_api, self._commands[command_argument].parser, args[0][1:])
         except Exception as e:
             # must be a local-import to get updated value
-            from conan.api.output import conan_output_level
-            if conan_output_level <= LEVEL_TRACE:
+            if ConanOutput.level_allowed(LEVEL_TRACE):
                 print(traceback.format_exc())
             self._conan2_migrate_recipe_msg(e)
             raise
 
     @staticmethod
     def _conan2_migrate_recipe_msg(exception):
         message = str(exception)
```

### Comparing `conan-2.0.4/conan/cli/command.py` & `conan-2.0.5/conan/cli/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import textwrap
 
+from conan.api.output import ConanOutput
 from conan.errors import ConanException
 
 
 class OnceArgument(argparse.Action):
     """Allows declaring a parameter that can have only one value, by default argparse takes the
     latest declared and it's very confusing.
     """
@@ -99,41 +100,17 @@
 class ConanArgumentParser(argparse.ArgumentParser):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def parse_args(self, args=None, namespace=None):
         args = super().parse_args(args)
-        self._process_log_level_args(args)
+        ConanOutput.define_log_level(args.v)
         return args
 
-    @staticmethod
-    def _process_log_level_args(args):
-        from conan.api import output
-        from conan.api.output import LEVEL_QUIET, LEVEL_ERROR, LEVEL_WARNING, LEVEL_NOTICE, \
-            LEVEL_STATUS, LEVEL_VERBOSE, LEVEL_DEBUG, LEVEL_TRACE
-
-        levels = {"quiet": LEVEL_QUIET,  # -vquiet 80
-                  "error": LEVEL_ERROR,  # -verror 70
-                  "warning": LEVEL_WARNING,  # -vwaring 60
-                  "notice": LEVEL_NOTICE,  # -vnotice 50
-                  "status": LEVEL_STATUS,  # -vstatus 40
-                  None: LEVEL_STATUS,  # -v 40
-                  "verbose": LEVEL_VERBOSE,  # -vverbose 30
-                  "debug": LEVEL_DEBUG,  # -vdebug 20
-                  "v": LEVEL_DEBUG,  # -vv 20
-                  "trace": LEVEL_TRACE,  # -vtrace 10
-                  "vv": LEVEL_TRACE,  # -vvv 10
-                  }
-
-        level = levels.get(args.v)
-        if not level:
-            raise ConanException(f"Invalid argument '-v{args.v}'")
-        output.conan_output_level = level
-
 
 class ConanCommand(BaseConanCommand):
     def __init__(self, method, group=None, formatters=None):
         super().__init__(method, formatters=formatters)
         self._subcommands = {}
         self._subcommand_parser = None
         self._group = group or "Other"
```

### Comparing `conan-2.0.4/conan/cli/commands/build.py` & `conan-2.0.5/conan/cli/commands/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,19 +25,20 @@
     add_lockfile_args(parser)
     args = parser.parse_args(*args)
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=True)
     folder = os.path.dirname(path)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
-
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
     print_profiles(profile_host, profile_build)
 
     deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                      args.user, args.channel,
                                                      profile_host, profile_build, lockfile, remotes,
                                                      args.update)
```

### Comparing `conan-2.0.4/conan/cli/commands/cache.py` & `conan-2.0.5/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/config.py` & `conan-2.0.5/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/create.py` & `conan-2.0.5/conan/cli/commands/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,29 @@
                         help='Alternative test folder name. By default it is "test_package". '
                              'Use "" to skip the test stage')
     args = parser.parse_args(*args)
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=True)
     test_conanfile_path = _get_test_conanfile_path(args.test_folder, path)
-
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     ref, conanfile = conan_api.export.export(path=path,
                                              name=args.name, version=args.version,
                                              user=args.user, channel=args.channel,
                                              lockfile=lockfile,
                                              remotes=remotes)
+
     # The package_type is not fully processed at export
     is_python_require = conanfile.package_type == "python-require"
     lockfile = conan_api.lockfile.update_lockfile_export(lockfile, conanfile, ref,
                                                          args.build_require)
 
     print_profiles(profile_host, profile_build)
 
@@ -72,14 +74,17 @@
                                                          lockfile=lockfile,
                                                          remotes=remotes, update=args.update)
         print_graph_basic(deps_graph)
         deps_graph.report_graph_error()
 
         # Not specified, force build the tested library
         build_modes = [ref.repr_notime()] if args.build is None else args.build
+        if args.build is None and conanfile.build_policy == "never":
+            raise ConanException(
+                "This package cannot be created, 'build_policy=never', it can only be 'export-pkg'")
         conan_api.graph.analyze_binaries(deps_graph, build_modes, remotes=remotes,
                                          update=args.update, lockfile=lockfile)
         print_graph_packages(deps_graph)
 
         conan_api.install.install_binaries(deps_graph=deps_graph, remotes=remotes)
         # We update the lockfile, so it will be updated for later ``test_package``
         lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
```

### Comparing `conan-2.0.4/conan/cli/commands/download.py` & `conan-2.0.5/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/editable.py` & `conan-2.0.5/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/export.py` & `conan-2.0.5/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/export_pkg.py` & `conan-2.0.5/conan/cli/commands/export_pkg.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,16 +39,18 @@
     add_lockfile_args(parser)
     add_profiles_args(parser)
     args = parser.parse_args(*args)
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=True)
     test_conanfile_path = _get_test_conanfile_path(args.test_folder, path)
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile, conanfile_path=path,
-                                               cwd=cwd, partial=args.lockfile_partial)
+                                               cwd=cwd, partial=args.lockfile_partial,
+                                               overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
 
     ref, conanfile = conan_api.export.export(path=path, name=args.name, version=args.version,
                                              user=args.user, channel=args.channel, lockfile=lockfile,
                                              remotes=remotes)
     # The package_type is not fully processed at export
```

### Comparing `conan-2.0.4/conan/cli/commands/graph.py` & `conan-2.0.5/conan/cli/commands/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,18 +47,20 @@
                              "--requires")
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=None) if args.path else None
 
     # Basic collaborators, remotes, lockfile, profiles
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     if path:
         deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.build, args.update)
@@ -73,16 +75,15 @@
     out = ConanOutput()
     out.title("Computing the build order")
     install_graph = InstallGraph(deps_graph)
     install_order_serialized = install_graph.install_build_order()
 
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
-    conanfile_path = os.path.dirname(deps_graph.root.path) if deps_graph.root.path else os.getcwd()
-    conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, conanfile_path)
+    conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
 
     return install_order_serialized
 
 
 @conan_subcommand(formatters={"text": cli_build_order, "json": json_build_order})
 def graph_build_order_merge(conan_api, parser, subparser, *args):
     """
@@ -112,15 +113,15 @@
     common_graph_args(subparser)
     subparser.add_argument("--check-updates", default=False, action="store_true",
                            help="Check if there are recipe updates")
     subparser.add_argument("--filter", action="append",
                            help="Show only the specified fields")
     subparser.add_argument("--package-filter", action="append",
                            help='Print information only for packages that match the patterns')
-    subparser.add_argument("--deploy", action="append",
+    subparser.add_argument("-d", "--deployer", action="append",
                            help='Deploy using the provided deployer to the output folder')
     subparser.add_argument("--build-require", action='store_true', default=False,
                            help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     # parameter validation
     validate_common_graph_args(args)
@@ -128,18 +129,20 @@
         raise ConanException(f"Formatted output '{args.format}' cannot filter fields")
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=None) if args.path else None
 
     # Basic collaborators, remotes, lockfile, profiles
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     if path:
         deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update,
@@ -160,16 +163,16 @@
         print_graph_packages(deps_graph)
 
         conan_api.install.install_system_requires(deps_graph, only_info=True)
         conan_api.install.install_sources(deps_graph, remotes=remotes)
 
         lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                       clean=args.lockfile_clean)
-        conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, os.getcwd())
-        if args.deploy:
+        conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
+        if args.deployer:
             base_folder = os.getcwd()
-            do_deploys(conan_api, deps_graph, args.deploy, base_folder)
+            do_deploys(conan_api, deps_graph, args.deployer, base_folder)
 
     return {"graph": deps_graph,
             "field_filter": args.filter,
             "package_filter": args.package_filter,
             "conan_api": conan_api}
```

### Comparing `conan-2.0.4/conan/cli/commands/install.py` & `conan-2.0.5/conan/cli/commands/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     generators.
     """
     common_graph_args(parser)
     parser.add_argument("-g", "--generator", action="append",
                         help='Generators to use')
     parser.add_argument("-of", "--output-folder",
                         help='The root output folder for generated and build files')
-    parser.add_argument("--deploy", action="append",
+    parser.add_argument("-d", "--deployer", action="append",
                         help='Deploy using the provided deployer to the output folder')
     parser.add_argument("--build-require", action='store_true', default=False,
                         help='Whether the provided reference is a build-require')
     args = parser.parse_args(*args)
 
     validate_common_graph_args(args)
     cwd = os.getcwd()
@@ -52,18 +52,20 @@
     if args.output_folder:
         output_folder = make_abs_path(args.output_folder, cwd)
     else:
         output_folder = None
 
     # Basic collaborators, remotes, lockfile, profiles
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
     print_profiles(profile_host, profile_build)
     if path:
         deps_graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                          args.user, args.channel,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update,
@@ -82,15 +84,15 @@
     conan_api.install.install_binaries(deps_graph=deps_graph, remotes=remotes)
 
     out.title("Finalizing install (deploy, generators)")
     conan_api.install.install_consumer(deps_graph=deps_graph,
                                        generators=args.generator,
                                        output_folder=output_folder,
                                        source_folder=source_folder,
-                                       deploy=args.deploy
+                                       deploy=args.deployer
                                        )
 
     out.success("Install finished successfully")
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
     return deps_graph
```

### Comparing `conan-2.0.4/conan/cli/commands/list.py` & `conan-2.0.5/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/lock.py` & `conan-2.0.5/conan/cli/commands/lock.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
     # parameter validation
     validate_common_graph_args(args)
 
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=None) if args.path else None
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile, conanfile_path=path,
-                                               cwd=cwd, partial=True)
+                                               cwd=cwd, partial=True, overrides=overrides)
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     if path:
         graph = conan_api.graph.load_graph_consumer(path, args.name, args.version,
                                                     args.user, args.channel,
                                                     profile_host, profile_build, lockfile,
                                                     remotes, args.build, args.update,
```

### Comparing `conan-2.0.4/conan/cli/commands/new.py` & `conan-2.0.5/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/profile.py` & `conan-2.0.5/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/remote.py` & `conan-2.0.5/conan/cli/commands/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,15 @@
     subparser.add_argument("--index", action=OnceArgument, type=int,
                            help="Insert the remote at a specific position in the remote list")
     subparser.add_argument("-f", "--force", action='store_true',
                            help="Force the definition of the remote even if duplicated")
     subparser.set_defaults(secure=True)
     args = parser.parse_args(*args)
     r = Remote(args.name, args.url, args.secure, disabled=False)
-    conan_api.remotes.add(r, force=args.force)
-    if args.index is not None:
-        conan_api.remotes.move(r, args.index)
+    conan_api.remotes.add(r, force=args.force, index=args.index)
 
 
 @conan_subcommand()
 def remote_remove(conan_api, parser, subparser, *args):
     """
     Remove a remote.
     """
@@ -104,34 +102,26 @@
                            help="Allow insecure server connections when using SSL")
     subparser.add_argument("--index", action=OnceArgument, type=int,
                            help="Insert the remote at a specific position in the remote list")
     subparser.set_defaults(secure=None)
     args = parser.parse_args(*args)
     if args.url is None and args.secure is None and args.index is None:
         subparser.error("Please add at least one argument to update")
-    r = conan_api.remotes.get(args.remote)
-    if args.url is not None:
-        r.url = args.url
-    if args.secure is not None:
-        r.verify_ssl = args.secure
-    conan_api.remotes.update(r)
-    if args.index is not None:
-        conan_api.remotes.move(r, args.index)
+    conan_api.remotes.update(args.remote, args.url, args.secure, index=args.index)
 
 
 @conan_subcommand()
 def remote_rename(conan_api, parser, subparser, *args):
     """
     Rename a remote.
     """
     subparser.add_argument("remote", help="Current name of the remote")
     subparser.add_argument("new_name", help="New name for the remote")
     args = parser.parse_args(*args)
-    r = conan_api.remotes.get(args.remote)
-    conan_api.remotes.rename(r, args.new_name)
+    conan_api.remotes.rename(args.remote, args.new_name)
 
 
 @conan_subcommand(formatters={"text": print_remote_list, "json": formatter_remote_list_json})
 def remote_enable(conan_api, parser, subparser, *args):
     """
     Enable all the remotes matching a pattern.
     """
```

### Comparing `conan-2.0.4/conan/cli/commands/remove.py` & `conan-2.0.5/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/search.py` & `conan-2.0.5/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/source.py` & `conan-2.0.5/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/commands/test.py` & `conan-2.0.5/conan/cli/commands/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,30 @@
     add_common_install_arguments(parser)
     add_lockfile_args(parser)
     args = parser.parse_args(*args)
 
     cwd = os.getcwd()
     ref = RecipeReference.loads(args.reference)
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=True)
+    overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
-                                               partial=args.lockfile_partial)
+                                               partial=args.lockfile_partial,
+                                               overrides=overrides)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
     profile_host, profile_build = conan_api.profiles.get_profiles_from_args(args)
 
     print_profiles(profile_host, profile_build)
 
     deps_graph = run_test(conan_api, path, ref, profile_host, profile_build, remotes, lockfile,
                           args.update, build_modes=args.build)
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
-    conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, os.path.dirname(path))
+    conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
 
 
 def run_test(conan_api, path, ref, profile_host, profile_build, remotes, lockfile, update,
              build_modes, tested_python_requires=None):
     root_node = conan_api.graph.load_root_test_conanfile(path, ref,
                                                          profile_host, profile_build,
                                                          remotes=remotes,
```

### Comparing `conan-2.0.4/conan/cli/commands/upload.py` & `conan-2.0.5/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/graph/graph.py` & `conan-2.0.5/conan/cli/formatters/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.0.5/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.0.5/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/list/binary_html_table.py` & `conan-2.0.5/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/list/list.py` & `conan-2.0.5/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/formatters/list/search_table_html.py` & `conan-2.0.5/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/cli/printers/graph.py` & `conan-2.0.5/conan/cli/printers/graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from conan.api.output import ConanOutput, Color
+from conan.api.output import ConanOutput, Color, LEVEL_VERBOSE
 from conans.client.graph.graph import RECIPE_CONSUMER, RECIPE_VIRTUAL, CONTEXT_BUILD, BINARY_SKIP,\
     BINARY_SYSTEM_TOOL
 
 
 def print_graph_basic(graph):
     # I am excluding the "download"-"cache" or remote information, that is not
     # the definition of the graph, but some history how it was computed
@@ -61,14 +61,20 @@
     _format_resolved("Resolved alias", graph.aliased)
     if graph.aliased:
         output.warning("'alias' is a Conan 1.X legacy feature, no longer recommended and "
                        "it might be removed in 3.0.")
         output.warning("Consider using version-ranges instead.")
     _format_resolved("Resolved version ranges", graph.resolved_ranges)
 
+    overrides = graph.overrides()
+    if overrides:
+        output.info("Overrides", Color.BRIGHT_YELLOW)
+        for req, override_info in overrides.serialize().items():
+            output.info("    {}: {}".format(req, override_info), Color.BRIGHT_CYAN)
+
     if deprecated:
         output.info("Deprecated", Color.BRIGHT_YELLOW)
         for d, reason in deprecated.items():
             reason = f": {reason}" if reason else ""
             output.info("    {}{}".format(d, reason), Color.BRIGHT_CYAN)
 
 
@@ -76,31 +82,45 @@
     # I am excluding the "download"-"cache" or remote information, that is not
     # the definition of the graph, but some history how it was computed
     # maybe we want to summarize that info after the "GraphBuilder" ends?
     output = ConanOutput()
     requires = {}
     build_requires = {}
     test_requires = {}
+    skipped_requires = []
+    tab = "    "
     for node in graph.nodes:
         if node.recipe in (RECIPE_CONSUMER, RECIPE_VIRTUAL):
             continue
         if node.context == CONTEXT_BUILD:
-            build_requires[node.pref] = node.binary, node.binary_remote
+            existing = build_requires.setdefault(node.pref, [node.binary, node.binary_remote])
         else:
             if node.test:
-                test_requires[node.pref] = node.binary, node.binary_remote
+                existing = test_requires.setdefault(node.pref, [node.binary, node.binary_remote])
             else:
-                requires[node.pref] = node.binary, node.binary_remote
+                existing = requires.setdefault(node.pref, [node.binary, node.binary_remote])
+        # TO avoid showing as "skip" something that is used in other node of the graph
+        if existing[0] == BINARY_SKIP:
+            existing[0] = node.binary
 
     def _format_requires(title, reqs_to_print):
         if not reqs_to_print:
             return
         output.info(title, Color.BRIGHT_YELLOW)
         for pref, (status, remote) in sorted(reqs_to_print.items(), key=repr):
-            if remote is not None and status != BINARY_SKIP:
-                status = "{} ({})".format(status, remote.name)
             name = pref.repr_notime() if status != BINARY_SYSTEM_TOOL else str(pref.ref)
-            output.info("    {} - {}".format(name, status), Color.BRIGHT_CYAN)
+            msg = f"{tab}{name} - {status}"
+            if remote is not None and status != BINARY_SKIP:
+                msg += f" ({remote.name})"
+            if status == BINARY_SKIP:
+                skipped_requires.append(str(pref.ref))
+                output.verbose(msg, Color.BRIGHT_CYAN)
+            else:
+                output.info(msg, Color.BRIGHT_CYAN)
 
     _format_requires("Requirements", requires)
     _format_requires("Test requirements", test_requires)
     _format_requires("Build requirements", build_requires)
+
+    if skipped_requires and not output.level_allowed(LEVEL_VERBOSE):
+        output.info("Skipped binaries", Color.BRIGHT_YELLOW)
+        output.info(f"{tab}{skipped_requires}", Color.BRIGHT_CYAN)
```

### Comparing `conan-2.0.4/conan/internal/api/new/autoools_exe.py` & `conan-2.0.5/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/autotools_lib.py` & `conan-2.0.5/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/basic.py` & `conan-2.0.5/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/bazel_exe.py` & `conan-2.0.5/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/bazel_lib.py` & `conan-2.0.5/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/cmake_exe.py` & `conan-2.0.5/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/cmake_lib.py` & `conan-2.0.5/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/meson_exe.py` & `conan-2.0.5/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/meson_lib.py` & `conan-2.0.5/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/msbuild_exe.py` & `conan-2.0.5/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/api/new/msbuild_lib.py` & `conan-2.0.5/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/cache/cache.py` & `conan-2.0.5/conan/internal/cache/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import hashlib
 import os
+import uuid
 
 from conan.internal.cache.conan_reference_layout import RecipeLayout, PackageLayout
 # TODO: Random folders are no longer accessible, how to get rid of them asap?
 # TODO: Add timestamp for LRU
 # TODO: We need the workflow to remove existing references.
 from conan.internal.cache.db.cache_database import CacheDatabase
 from conans.errors import ConanReferenceAlreadyExistsInDB, ConanReferenceDoesNotExistInDB
@@ -52,16 +53,19 @@
         # The reference will not have revision, but it will be always constant
         h = ref.name[:5] + DataCache._short_hash_path(ref.repr_notime())
         return os.path.join("t", h)
 
     @staticmethod
     def _get_tmp_path_pref(pref):
         # The reference will not have revision, but it will be always constant
-        h = pref.ref.name[:5] + DataCache._short_hash_path(pref.repr_notime())
-        return os.path.join("t", h)
+        assert pref.revision is None
+        assert pref.timestamp is None
+        random_id = str(uuid.uuid4())
+        h = pref.ref.name[:5] + DataCache._short_hash_path(pref.repr_notime() + random_id)
+        return os.path.join("b", h)
 
     @staticmethod
     def _get_path(ref: RecipeReference):
         return ref.name[:5] + DataCache._short_hash_path(ref.repr_notime())
 
     @staticmethod
     def _get_path_pref(pref):
@@ -169,39 +173,33 @@
         return self._db.get_package_timestamp(pref)
 
     def remove_recipe(self, layout: RecipeLayout):
         layout.remove()
         # FIXME: This is clearing package binaries from DB, but not from disk/layout
         self._db.remove_recipe(layout.reference)
 
-    def remove_package(self, layout: RecipeLayout):
+    def remove_package(self, layout: PackageLayout):
         layout.remove()
         self._db.remove_package(layout.reference)
 
     def assign_prev(self, layout: PackageLayout):
         pref = layout.reference
 
-        new_path = self._get_path_pref(pref)
-
-        full_path = self._full_path(new_path)
-        rmdir(full_path)
-
-        renamedir(self._full_path(layout.base_folder), full_path)
-        layout._base_folder = os.path.join(self.base_folder, new_path)
-
         build_id = layout.build_id
         pref.timestamp = revision_timestamp_now()
         # Wait until it finish to really update the DB
+        relpath = os.path.relpath(layout.base_folder, self.base_folder)
         try:
-            self._db.create_package(new_path, pref, build_id)
+            self._db.create_package(relpath, pref, build_id)
         except ConanReferenceAlreadyExistsInDB:
+            # TODO: Optimize this into 1 single UPSERT operation
             # This was exported before, making it latest again, update timestamp
-            self._db.update_package_timestamp(pref)
-
-        return new_path
+            pkg_layout = self.get_package_layout(pref)
+            pkg_layout.remove()
+            self._db.update_package_timestamp(pref, path=relpath)
 
     def assign_rrev(self, layout: RecipeLayout):
         """ called at export, once the exported recipe revision has been computed, it
         can register for the first time the new RecipeReference"""
         ref = layout.reference
         assert ref.revision is not None, "Revision must exist after export"
         assert ref.timestamp is None, "Timestamp no defined yet"
```

### Comparing `conan-2.0.4/conan/internal/cache/conan_reference_layout.py` & `conan-2.0.5/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/cache/db/cache_database.py` & `conan-2.0.5/conan/internal/cache/db/cache_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     def get_latest_package_reference(self, ref):
         prevs = self.get_package_revisions_references(ref, True)
         return prevs[0] if prevs else None
 
     def update_recipe_timestamp(self, ref):
         self._recipes.update_timestamp(ref)
 
-    def update_package_timestamp(self, pref: PkgReference):
-        self._packages.update_timestamp(pref)
+    def update_package_timestamp(self, pref: PkgReference, path: str):
+        self._packages.update_timestamp(pref, path=path)
 
     def remove_recipe(self, ref: RecipeReference):
         # Removing the recipe must remove all the package binaries too from DB
         self._recipes.remove(ref)
         self._packages.remove_recipe(ref)
 
     def remove_package(self, ref: PkgReference):
```

### Comparing `conan-2.0.4/conan/internal/cache/db/packages_table.py` & `conan-2.0.5/conan/internal/cache/db/packages_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,19 +78,19 @@
                 conn.execute(f'INSERT INTO {self.table_name} '
                                    f'VALUES ({placeholders})',
                                    [str(pref.ref), pref.ref.revision, pref.package_id, pref.revision,
                                     path, pref.timestamp, build_id])
             except sqlite3.IntegrityError:
                 raise ConanReferenceAlreadyExistsInDB(f"Reference '{repr(pref)}' already exists")
 
-    def update_timestamp(self, pref: PkgReference):
+    def update_timestamp(self, pref: PkgReference, path: str):
         assert pref.revision
         assert pref.timestamp
         where_clause = self._where_clause(pref)
-        set_clause = self._set_clause(pref)
+        set_clause = self._set_clause(pref, path=path)
         query = f"UPDATE {self.table_name} " \
                 f"SET {set_clause} " \
                 f"WHERE {where_clause};"
         with self.db_connection() as conn:
             try:
                 conn.execute(query)
             except sqlite3.IntegrityError:
```

### Comparing `conan-2.0.4/conan/internal/cache/db/recipes_table.py` & `conan-2.0.5/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/cache/db/table.py` & `conan-2.0.5/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/conan_app.py` & `conan-2.0.5/conan/internal/conan_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from conan.api.output import ConanOutput
 from conans.client.cache.cache import ClientCache
 from conans.client.graph.proxy import ConanProxy
 from conans.client.graph.python_requires import PyRequireLoader
 from conans.client.graph.range_resolver import RangeResolver
 from conans.client.hook_manager import HookManager
 from conans.client.loader import ConanFileLoader, load_python_file
 from conans.client.remote_manager import RemoteManager
@@ -40,14 +41,15 @@
 
         self.cache_folder = cache_folder
         self.cache = ClientCache(self.cache_folder)
 
         self.hook_manager = HookManager(self.cache.hooks_path)
         # Wraps an http_requester to inject proxies, certs, etc
         global_conf = self.cache.new_config
+        ConanOutput.define_silence_warnings(global_conf.get("core:skip_warnings", check_type=list))
         self.requester = ConanRequester(global_conf, cache_folder)
         # To handle remote connections
         rest_client_factory = RestApiClientFactory(self.requester, global_conf)
         # Wraps RestApiClient to add authentication support (same interface)
         auth_manager = ConanApiAuthManager(rest_client_factory, self.cache)
         # Handle remote connections
         self.remote_manager = RemoteManager(self.cache, auth_manager)
```

### Comparing `conan-2.0.4/conan/internal/deploy.py` & `conan-2.0.5/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/internal/integrity_check.py` & `conan-2.0.5/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/android/utils.py` & `conan-2.0.5/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/apple/__init__.py` & `conan-2.0.5/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/apple/apple.py` & `conan-2.0.5/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/apple/xcodebuild.py` & `conan-2.0.5/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/apple/xcodedeps.py` & `conan-2.0.5/conan/tools/apple/xcodedeps.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,17 +202,18 @@
 
     def _all_xconfig_file(self, deps, content):
         """
         this is a .xcconfig file including all declared dependencies
         """
         content_multi = content or self._all_xconfig
 
-        for req, dep in deps.items():
-            dep_name = _format_name(dep.ref.name)
-            content_multi = content_multi + '\n#include "conan_{}.xcconfig"\n'.format(dep_name)
+        for dep in deps.values():
+            include_file = f'conan_{_format_name(dep.ref.name)}.xcconfig'
+            if include_file not in content_multi:
+                content_multi = content_multi + f'\n#include "{include_file}"\n'
         return content_multi
 
     def _pkg_xconfig_file(self, components):
         """
         this is a .xcconfig file including the components for each package
         """
         content_multi = self._pkg_xconfig
@@ -297,16 +298,17 @@
                                                                        pkg_folder,
                                                                        transitive_internal,
                                                                        transitive_external)
                     include_components_names.append((dep_name, comp_name))
                     result.update(component_content)
             else:
                 public_deps = []
+                transitive_requires = [r for r, _ in get_transitive_requires(self._conanfile, dep).items()]
                 for r, d in dep.dependencies.direct_host.items():
-                    if not r.visible:
+                    if r not in transitive_requires:
                         continue
                     if d.cpp_info.has_components:
                         sorted_components = d.cpp_info.get_sorted_components().items()
                         for comp_name, comp_cpp_info in sorted_components:
                             public_deps.append((_format_name(d.ref.name), _format_name(comp_name)))
                     else:
                         public_deps.append((_format_name(d.ref.name),) * 2)
```

### Comparing `conan-2.0.4/conan/tools/apple/xcodetoolchain.py` & `conan-2.0.5/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/build/__init__.py` & `conan-2.0.5/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/build/cppstd.py` & `conan-2.0.5/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/build/cpu.py` & `conan-2.0.5/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/build/cross_building.py` & `conan-2.0.5/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/build/flags.py` & `conan-2.0.5/conan/tools/build/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
             # Modules/Compiler/SunPro-CXX.cmake
             flags = {"Debug": ["-g"],
                      "Release": ["-xO3"],
                      "RelWithDebInfo": ["-xO2", "-g"],
                      "MinSizeRel": ["-xO2", "-xspace"],
                      }.get(build_type, [])
             return flags
-    return ""
+    return []
 
 
 def cppstd_flag(settings):
     compiler = settings.get_safe("compiler")
     compiler_version = settings.get_safe("compiler.version")
     cppstd = settings.get_safe("compiler.cppstd")
```

### Comparing `conan-2.0.4/conan/tools/build/stdcpp_library.py` & `conan-2.0.5/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmake.py` & `conan-2.0.5/conan/tools/cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -40,16 +40,23 @@
     def render(self):
         try:
             context = self.context
         except Exception as e:
             raise ConanException("error generating context for '{}': {}".format(self.conanfile, e))
         if context is None:
             return
-        return Template(self.template, trim_blocks=True, lstrip_blocks=True,
-                        undefined=jinja2.StrictUndefined).render(context)
+
+        # Cache the template instance as a class attribute to greatly speed up the rendering
+        # NOTE: this assumes that self.template always returns the same string
+        template_instance = getattr(type(self), "template_instance", None)
+        if template_instance is None:
+            template_instance = Template(self.template, trim_blocks=True, lstrip_blocks=True,
+                                         undefined=jinja2.StrictUndefined)
+            setattr(type(self), "template_instance", template_instance)
+        return template_instance.render(context)
 
     def context(self):
         raise NotImplementedError()
 
     @property
     def template(self):
         raise NotImplementedError()
```

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,34 +63,32 @@
                                   NO_DEFAULT_PATH NO_CMAKE_FIND_ROOT_PATH)
                      if(NOT CONAN_SHARED_FOUND_LIBRARY)
                        message(STATUS "Cannot locate shared library: ${_LIBRARY_NAME}")
                        message(DEBUG "DLL library not found, creating UNKNOWN IMPORTED target")
                        if(NOT TARGET ${_LIB_NAME})
                           add_library(${_LIB_NAME} UNKNOWN IMPORTED)
                        endif()
-                       set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION ${CONAN_FOUND_LIBRARY})
+                       set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION${config_suffix} ${CONAN_FOUND_LIBRARY})
                      else()
                         if(NOT TARGET ${_LIB_NAME})
                           add_library(${_LIB_NAME} SHARED IMPORTED)
                         endif()
-                        set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION ${CONAN_SHARED_FOUND_LIBRARY})
-                        set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_IMPLIB ${CONAN_FOUND_LIBRARY})
+                        set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION${config_suffix} ${CONAN_SHARED_FOUND_LIBRARY})
+                        set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_IMPLIB${config_suffix} ${CONAN_FOUND_LIBRARY})
                         message(DEBUG "Found DLL and STATIC at ${CONAN_SHARED_FOUND_LIBRARY}, ${CONAN_FOUND_LIBRARY}")
                      endif()
                      unset(CONAN_SHARED_FOUND_LIBRARY CACHE)
                    else()
                      if(NOT TARGET ${_LIB_NAME})
                          # library_type can be STATIC, still UNKNOWN (if no package type available in the recipe) or SHARED (but no windows)
                          add_library(${_LIB_NAME} ${library_type} IMPORTED)
                      endif()
                      message(DEBUG "Created target ${_LIB_NAME} ${library_type} IMPORTED")
-                     set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION ${CONAN_FOUND_LIBRARY} IMPORTED_NO_SONAME ${no_soname_mode})
+                     set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION${config_suffix} ${CONAN_FOUND_LIBRARY} IMPORTED_NO_SONAME ${no_soname_mode})
                    endif()
-                   # Link library file
-                   set_target_properties(${_LIB_NAME} PROPERTIES IMPORTED_LOCATION${config_suffix} ${CONAN_FOUND_LIBRARY})
                    list(APPEND _out_libraries_target ${_LIB_NAME})
                    message(VERBOSE "Conan: Found: ${CONAN_FOUND_LIBRARY}")
                else()
                    message(FATAL_ERROR "Library '${_LIBRARY_NAME}' not found in package. If '${_LIBRARY_NAME}' is a system library, declare it with 'cpp_info.system_libs' property")
                endif()
                unset(CONAN_FOUND_LIBRARY CACHE)
            endforeach()
```

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/file_api.py` & `conan-2.0.5/conan/tools/cmake/file_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/layout.py` & `conan-2.0.5/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/presets.py` & `conan-2.0.5/conan/tools/cmake/presets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/cmake/toolchain/blocks.py` & `conan-2.0.5/conan/tools/cmake/toolchain/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,14 +714,15 @@
     def _get_generic_system_name(self):
         os_host = self._conanfile.settings.get_safe("os")
         os_build = self._conanfile.settings_build.get_safe("os")
         arch_host = self._conanfile.settings.get_safe("arch")
         arch_build = self._conanfile.settings_build.get_safe("arch")
         cmake_system_name_map = {"Neutrino": "QNX",
                                  "": "Generic",
+                                 "baremetal": "Generic",
                                  None: "Generic"}
         if os_host != os_build:
             return cmake_system_name_map.get(os_host, os_host)
         elif arch_host is not None and arch_host != arch_build:
             if not ((arch_build == "x86_64") and (arch_host == "x86") or
                     (arch_build == "sparcv9") and (arch_host == "sparc") or
                     (arch_build == "ppc64") and (arch_host == "ppc32")):
```

### Comparing `conan-2.0.4/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.0.5/conan/tools/cmake/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/env/environment.py` & `conan-2.0.5/conan/tools/env/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,14 @@
             @echo off
             chcp 65001 > nul
             {deactivate}
             """).format(deactivate=deactivate if generate_deactivate else "")
         result = [capture]
         for varname, varvalues in self._values.items():
             value = varvalues.get_str("%{name}%", subsystem=self._subsystem, pathsep=self._pathsep)
-            # To make the script relocatable
             result.append('set "{}={}"'.format(varname, value))
 
         content = "\n".join(result)
         content = relativize_generated_file(content, self._conanfile, "%~dp0")
         # It is very important to save it correctly with utf-8, the Conan util save() is broken
         os.makedirs(os.path.dirname(os.path.abspath(file_location)), exist_ok=True)
         open(file_location, "w", encoding="utf-8").write(content)
@@ -497,14 +496,16 @@
             value = value.replace('"', '\\"')
             if value:
                 result.append('export {}="{}"'.format(varname, value))
             else:
                 result.append('unset {}'.format(varname))
 
         content = "\n".join(result)
+        content = relativize_generated_file(content, self._conanfile, "$script_folder")
+        content = f'script_folder="{os.path.abspath(filepath)}"\n' + content
         save(file_location, content)
 
     def save_script(self, filename):
         """
         Saves a script file (bat, sh, ps1) with a launcher to set the environment.
         If the conf "tools.env.virtualenv:powershell" is set to True it will generate powershell
         launchers if Windows.
```

### Comparing `conan-2.0.4/conan/tools/env/virtualbuildenv.py` & `conan-2.0.5/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/env/virtualrunenv.py` & `conan-2.0.5/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/__init__.py` & `conan-2.0.5/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/conandata.py` & `conan-2.0.5/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/copy_pattern.py` & `conan-2.0.5/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/cpp_package.py` & `conan-2.0.5/conan/tools/files/cpp_package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/files.py` & `conan-2.0.5/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/packager.py` & `conan-2.0.5/conan/tools/files/packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
         self.patterns.build.include = ["*.h", "*.hpp", "*.hxx"]
         self.patterns.build.lib = ["*.so", "*.so.*", "*.a", "*.lib", "*.dylib"]
         self.patterns.build.bin = ["*.exe", "*.dll"]
 
     def run(self):
         cf = self._conanfile
         # Check that the components declared in source/build are in package
-        cnames = set(cf.cpp.source.component_names)
-        cnames = cnames.union(set(cf.cpp.build.component_names))
-        if cnames.difference(set(cf.cpp.package.component_names)):
+        cnames = set(cf.cpp.source.components)
+        cnames = cnames.union(set(cf.cpp.build.components))
+        if cnames.difference(set(cf.cpp.package.components)):
             # TODO: Raise? Warning? Ignore?
             raise ConanException("There are components declared in cpp.source.components"
                                  " or in cpp.build.components that are not declared in"
                                  " cpp.package.components")
         if cnames:
             for cname in cnames:
                 if cname in cf.cpp.source.components:
```

### Comparing `conan-2.0.4/conan/tools/files/patches.py` & `conan-2.0.5/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/files/symlinks/symlinks.py` & `conan-2.0.5/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/autotools.py` & `conan-2.0.5/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/autotoolsdeps.py` & `conan-2.0.5/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.0.5/conan/tools/gnu/autotoolstoolchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from conan.tools.apple.apple import apple_min_version_flag, is_apple_os, to_apple_arch, apple_sdk_path
 from conan.tools.apple.apple import get_apple_sdk_fullname
 from conan.tools.build import cmd_args_to_string, save_toolchain_args
 from conan.tools.build.cross_building import cross_building
 from conan.tools.build.flags import architecture_flag, build_type_flags, cppstd_flag, build_type_link_flags, libcxx_flags
 from conan.tools.env import Environment
 from conan.tools.gnu.get_gnu_triplet import _get_gnu_triplet
-from conan.tools.microsoft import VCVars, msvc_runtime_flag
+from conan.tools.microsoft import VCVars, msvc_runtime_flag, unix_path
 from conans.errors import ConanException
 from conans.model.pkg_type import PackageType
 
 
 class AutotoolsToolchain:
     def __init__(self, conanfile, namespace=None, prefix="/"):
         """
@@ -148,15 +148,18 @@
     def environment(self):
         env = Environment()
         compilers_by_conf = self._conanfile.conf.get("tools.build:compiler_executables", default={}, check_type=dict)
         if compilers_by_conf:
             compilers_mapping = {"c": "CC", "cpp": "CXX", "cuda": "NVCC", "fortran": "FC"}
             for comp, env_var in compilers_mapping.items():
                 if comp in compilers_by_conf:
-                    env.define(env_var, compilers_by_conf[comp])
+                    compiler = compilers_by_conf[comp]
+                    # https://github.com/conan-io/conan/issues/13780
+                    compiler = unix_path(self._conanfile, compiler)
+                    env.define(env_var, compiler)
         env.append("CPPFLAGS", ["-D{}".format(d) for d in self.defines])
         env.append("CXXFLAGS", self.cxxflags)
         env.append("CFLAGS", self.cflags)
         env.append("LDFLAGS", self.ldflags)
         env.prepend_path("PKG_CONFIG_PATH", self._conanfile.generators_folder)
         return env
```

### Comparing `conan-2.0.4/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.0.5/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/gnudeps_flags.py` & `conan-2.0.5/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/pkgconfig.py` & `conan-2.0.5/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.0.5/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/google/bazel.py` & `conan-2.0.5/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/google/bazeldeps.py` & `conan-2.0.5/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/google/layout.py` & `conan-2.0.5/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/google/toolchain.py` & `conan-2.0.5/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/intel/intel_cc.py` & `conan-2.0.5/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/layout/__init__.py` & `conan-2.0.5/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/meson/helpers.py` & `conan-2.0.5/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/meson/meson.py` & `conan-2.0.5/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/meson/toolchain.py` & `conan-2.0.5/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/__init__.py` & `conan-2.0.5/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/layout.py` & `conan-2.0.5/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/msbuild.py` & `conan-2.0.5/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/msbuilddeps.py` & `conan-2.0.5/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/nmakedeps.py` & `conan-2.0.5/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.0.5/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/subsystems.py` & `conan-2.0.5/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/toolchain.py` & `conan-2.0.5/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/microsoft/visual.py` & `conan-2.0.5/conan/tools/microsoft/visual.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/premake/premake.py` & `conan-2.0.5/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/premake/premakedeps.py` & `conan-2.0.5/conan/tools/premake/premakedeps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import itertools 
+import itertools
 import glob
 import re
 
 from conan.internal import check_duplicated_generator
-from conans.model.build_info import CppInfo
 from conans.util.files import save
 
 # Filename format strings
 PREMAKE_VAR_FILE = "conan_{pkgname}_vars{config}.premake5.lua"
 PREMAKE_CONF_FILE = "conan_{pkgname}{config}.premake5.lua"
 PREMAKE_PKG_FILE = "conan_{pkgname}.premake5.lua"
 PREMAKE_ROOT_FILE = "conandeps.premake5.lua"
@@ -80,42 +79,39 @@
     conan_setup_link(conf, pkg)
 end
 """
 
 
 # Helper class that expands cpp_info meta information in lua readable string sequences
 class _PremakeTemplate(object):
-    def __init__(self, deps_cpp_info):
-        self.includedirs = ",\n".join('"%s"' % p.replace("\\", "/")
-                                      for p in
-                                      deps_cpp_info.includedirs) if deps_cpp_info.includedirs else ""
-        self.libdirs = ",\n".join('"%s"' % p.replace("\\", "/")
-                                  for p in deps_cpp_info.libdirs) if deps_cpp_info.libdirs else ""
-        self.bindirs = ",\n".join('"%s"' % p.replace("\\", "/")
-                                  for p in deps_cpp_info.bindirs) if deps_cpp_info.bindirs else ""
-        self.libs = ", ".join(
-            '"%s"' % p.replace('"', '\\"') for p in deps_cpp_info.libs) if deps_cpp_info.libs else ""
-        self.system_libs = ", ".join('"%s"' % p.replace('"', '\\"') for p in
-                                     deps_cpp_info.system_libs) if deps_cpp_info.system_libs else ""
-        self.defines = ", ".join('"%s"' % p.replace('"', '\\"') for p in
-                                 deps_cpp_info.defines) if deps_cpp_info.defines else ""
-        self.cxxflags = ", ".join(
-            '"%s"' % p for p in deps_cpp_info.cxxflags) if deps_cpp_info.cxxflags else ""
-        self.cflags = ", ".join(
-            '"%s"' % p for p in deps_cpp_info.cflags) if deps_cpp_info.cflags else ""
-        self.sharedlinkflags = ", ".join('"%s"' % p.replace('"', '\\"') for p in
-                                         deps_cpp_info.sharedlinkflags) \
-            if deps_cpp_info.sharedlinkflags else ""
-        self.exelinkflags = ", ".join('"%s"' % p.replace('"', '\\"') for p in
-                                      deps_cpp_info.exelinkflags) \
-            if deps_cpp_info.exelinkflags else ""
+    def __init__(self, dep_cpp_info, pkg_folder):
+        def _format_paths(paths):
+            if not paths:
+                return ""
+            return ",\n".join(f'"{pkg_folder}/{p}"'.replace("\\", "/") for p in paths)
+
+        def _format_flags(flags):
+            if not flags:
+                return ""
+            return ", ".join('"%s"' % p.replace('"', '\\"') for p in flags)
+
+        self.includedirs = _format_paths(dep_cpp_info.includedirs)
+        self.libdirs = _format_paths(dep_cpp_info.libdirs)
+        self.bindirs = _format_paths(dep_cpp_info.bindirs)
+        self.libs = _format_flags(dep_cpp_info.libs)
+        self.system_libs = _format_flags(dep_cpp_info.system_libs)
+        self.defines = _format_flags(dep_cpp_info.defines)
+        self.cxxflags = _format_flags(dep_cpp_info.cxxflags)
+        self.cflags = _format_flags(dep_cpp_info.cflags)
+        self.sharedlinkflags = _format_flags(dep_cpp_info.sharedlinkflags)
+        self.exelinkflags = _format_flags(dep_cpp_info.exelinkflags)
         self.frameworks = ", ".join('"%s.framework"' % p.replace('"', '\\"') for p in
-                                    deps_cpp_info.frameworks) if deps_cpp_info.frameworks else ""
-        self.sysroot = "%s" % deps_cpp_info.sysroot.replace("\\",
-                                                            "/") if deps_cpp_info.sysroot else ""
+                                    dep_cpp_info.frameworks) if dep_cpp_info.frameworks else ""
+        self.sysroot = f"{pkg_folder}/{dep_cpp_info.sysroot}".replace("\\", "/") \
+            if dep_cpp_info.sysroot else ""
 
 
 class PremakeDeps(object):
     """
     PremakeDeps class generator
     conandeps.premake5.lua: unconditional import of all *direct* dependencies only
     """
@@ -149,27 +145,27 @@
             save(generator_file, content)
 
     def _config_suffix(self):
         props = [("Configuration", self.configuration),
                  ("Platform", self.architecture)]
         name = "".join("_%s" % v for _, v in props)
         return name.lower()
-    
+
     def _output_lua_file(self, filename, content):
         self.output_files[filename] = "\n".join(["#!lua", *content])
 
     def _indent_string(self, string, indent=1):
         return "\n".join([
             f"{self.tab * indent}{line}" for line in list(filter(None, string.splitlines()))
         ])
-    
+
     def _premake_filtered(self, content, configuration, architecture, indent=0):
         """
         - Surrounds the lua line(s) contained within ``content`` with a premake "filter" and returns the result.
-        - A "filter" will affect all premake function calls after it's set. It's used to limit following project 
+        - A "filter" will affect all premake function calls after it's set. It's used to limit following project
           setup function call(s) to a certain scope. Here it is used to limit the calls in content to only apply
           if the premake ``configuration`` and ``architecture`` matches the parameters in this function call.
         """
         lines = list(itertools.chain.from_iterable([cnt.splitlines() for cnt in content]))
         return [
             # Set new filter
             f'{self.tab * indent}filter {{ "configurations:{configuration}", "architecture:{architecture}" }}',
@@ -178,19 +174,19 @@
             # Clear active filter
             f"{self.tab * indent}filter {{}}",
         ]
 
     @property
     def content(self):
         check_duplicated_generator(self, self._conanfile)
-        
+
         self.output_files = {}
         conf_suffix = str(self._config_suffix())
         conf_name = conf_suffix[1::]
-        
+
         # Global utility file
         self._output_lua_file("conanutils.premake5.lua", [PREMAKE_TEMPLATE_UTILS])
 
         # Extract all dependencies
         host_req = self._conanfile.dependencies.host
         test_req = self._conanfile.dependencies.test
         build_req = self._conanfile.dependencies.build
@@ -205,23 +201,21 @@
         dep_names = []
         config_sets = []
         for require, dep in full_req:
             dep_name = require.ref.name
             dep_names.append(dep_name)
 
             # Convert and aggregate dependency's
-            dep_cppinfo = dep.cpp_info.copy()
-            dep_cppinfo.set_relative_base_folder(dep.package_folder)
-            dep_aggregate = dep_cppinfo.aggregated_components()
-            
+            dep_aggregate = dep.cpp_info.aggregated_components()
+
             # Generate config dependent package variable and setup premake file
             var_filename = PREMAKE_VAR_FILE.format(pkgname=dep_name, config=conf_suffix)
             self._output_lua_file(var_filename, [
-                PREMAKE_TEMPLATE_VAR.format(pkgname=dep_name, 
-                    config=conf_name, deps=_PremakeTemplate(dep_aggregate))
+                PREMAKE_TEMPLATE_VAR.format(pkgname=dep_name,
+                    config=conf_name, deps=_PremakeTemplate(dep_aggregate, dep.package_folder))
             ])
 
             # Create list of all available profiles by searching on disk
             file_pattern = PREMAKE_VAR_FILE.format(pkgname=dep_name, config="_*")
             file_regex = PREMAKE_VAR_FILE.format(pkgname=re.escape(dep_name), config="_(([^_]*)_(.*))")
             available_files = glob.glob(file_pattern)
             # Add filename of current generations var file if not already present
@@ -238,31 +232,31 @@
             pkg_filename = PREMAKE_PKG_FILE.format(pkgname=dep_name)
             pkg_files.append(pkg_filename)
             self._output_lua_file(pkg_filename, [
                 # Includes
                 *['include "{}"'.format(profile[0]) for profile in profiles],
             ])
 
-        # Output global premake file 
+        # Output global premake file
         self._output_lua_file(PREMAKE_ROOT_FILE, [
             # Includes
             *[f'include "{pkg_file}"' for pkg_file in pkg_files],
             # Functions
             PREMAKE_TEMPLATE_ROOT_FUNCTION.format(
-                function_name="conan_setup_build", 
-                lua_content=PREMAKE_TEMPLATE_ROOT_BUILD, 
+                function_name="conan_setup_build",
+                lua_content=PREMAKE_TEMPLATE_ROOT_BUILD,
                 filter_call="\n".join(
                     ["\n".join(self._premake_filtered(
                         [f'conan_setup_build("{config}")'], config.split("_", 1)[0], config.split("_", 1)[1], 2)
                     ) for config in config_sets]
                 )
             ),
             PREMAKE_TEMPLATE_ROOT_FUNCTION.format(
-                function_name="conan_setup_link", 
-                lua_content=PREMAKE_TEMPLATE_ROOT_LINK, 
+                function_name="conan_setup_link",
+                lua_content=PREMAKE_TEMPLATE_ROOT_LINK,
                 filter_call="\n".join(
                     ["\n".join(self._premake_filtered(
                         [f'conan_setup_link("{config}")'], config.split("_", 1)[0], config.split("_", 1)[1], 2)
                     ) for config in config_sets]
                 )
             ),
             PREMAKE_TEMPLATE_ROOT_GLOBAL
```

### Comparing `conan-2.0.4/conan/tools/qbs/qbs.py` & `conan-2.0.5/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/qbs/qbsprofile.py` & `conan-2.0.5/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/scm/git.py` & `conan-2.0.5/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan/tools/system/package_manager.py` & `conan-2.0.5/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conan.egg-info/PKG-INFO` & `conan-2.0.5/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.4
+Version: 2.0.5
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.4/conan.egg-info/SOURCES.txt` & `conan-2.0.5/conan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/cache/cache.py` & `conan-2.0.5/conans/client/cache/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import platform
+import textwrap
 from typing import List
 
 import yaml
 from jinja2 import FileSystemLoader, Environment
 
 from conan import conan_version
+from conan.api.output import ConanOutput
 from conan.internal.cache.cache import DataCache, RecipeLayout, PackageLayout
 from conans.client.cache.editable import EditablePackages
 from conans.client.cache.remote_registry import RemoteRegistry
 from conans.client.conf import default_settings_yml
 from conans.client.store.localdb import LocalDB
 from conans.errors import ConanException
 from conans.model.conf import ConfDefinition
@@ -23,16 +25,14 @@
 CONAN_SETTINGS = "settings.yml"
 LOCALDB = ".conan.db"
 REMOTES = "remotes.json"
 PROFILES_FOLDER = "profiles"
 EXTENSIONS_FOLDER = "extensions"
 HOOKS_EXTENSION_FOLDER = "hooks"
 PLUGINS_FOLDER = "plugins"
-DEPLOYERS_EXTENSION_FOLDER = "deploy"
-CUSTOM_COMMANDS_FOLDER = "commands"
 
 
 # TODO: Rename this to ClientHome
 class ClientCache(object):
     """ Class to represent/store/compute all the paths involved in the execution
     of conans commands. Accesses to real disk and reads/write things. (OLD client ConanPaths)
     """
@@ -54,14 +54,18 @@
     @property
     def temp_folder(self):
         """ temporary folder where Conan puts exports and packages before the final revision
         is computed"""
         # TODO: Improve the path definitions, this is very hardcoded
         return os.path.join(self.cache_folder, "p", "t")
 
+    @property
+    def builds_folder(self):
+        return os.path.join(self.cache_folder, "p", "b")
+
     def create_export_recipe_layout(self, ref: RecipeReference):
         return self._data_cache.create_export_recipe_layout(ref)
 
     def assign_rrev(self, layout: RecipeLayout):
         return self._data_cache.assign_rrev(layout)
 
     def create_build_pkg_layout(self, ref):
@@ -163,16 +167,24 @@
                 distro = None
                 if platform.system() in ["Linux", "FreeBSD"]:
                     import distro
                 template = Environment(loader=FileSystemLoader(self.cache_folder)).from_string(text)
                 content = template.render({"platform": platform, "os": os, "distro": distro,
                                            "conan_version": conan_version,
                                            "conan_home_folder": self.cache_folder})
-
                 self._new_config.loads(content)
+            else:  # creation of a blank global.conf file for user convenience
+                default_global_conf = textwrap.dedent("""\
+                    # Core configuration (type 'conan config list' to list possible values)
+                    # e.g, for CI systems, to raise if user input would block
+                    # core:non_interactive = True
+                    # some tools.xxx config also possible, though generally better in profiles
+                    # tools.android:ndk_path = my/path/to/android/ndk
+                    """)
+                save(self.new_config_path, default_global_conf)
         return self._new_config
 
     @property
     def localdb(self):
         localdb_filename = os.path.join(self.cache_folder, LOCALDB)
         return LocalDB.create(localdb_filename)
 
@@ -182,35 +194,41 @@
 
     @property
     def settings_path(self):
         return os.path.join(self.cache_folder, CONAN_SETTINGS)
 
     @property
     def custom_commands_path(self):
-        return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, CUSTOM_COMMANDS_FOLDER)
+        return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, "commands")
+
+    @property
+    def custom_generators_path(self):
+        return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, "generators")
 
     @property
     def plugins_path(self):
         return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, PLUGINS_FOLDER)
 
     @property
     def default_profile_path(self):
         # Used only in testing, and this class "reset_default_profile"
         return os.path.join(self.cache_folder, PROFILES_FOLDER, DEFAULT_PROFILE_NAME)
 
     @property
     def hooks_path(self):
-        """
-        :return: Hooks folder in client cache
-        """
         return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, HOOKS_EXTENSION_FOLDER)
 
     @property
     def deployers_path(self):
-        return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, DEPLOYERS_EXTENSION_FOLDER)
+        deploy = os.path.join(self.cache_folder, EXTENSIONS_FOLDER, "deploy")
+        if os.path.exists(deploy):
+            ConanOutput().warning("Use 'deployers' cache folder for deployers instead of 'deploy'",
+                                  warn_tag="deprecated")
+            return deploy
+        return os.path.join(self.cache_folder, EXTENSIONS_FOLDER, "deployers")
 
     @property
     def settings(self):
         """Returns {setting: [value, ...]} defining all the possible
            settings without values"""
         self.initialize_settings()
 
@@ -238,18 +256,15 @@
                         d[k] = appending_recursive_dict_update(current, v)
                     else:
                         d[k] = v
                 return d
 
             appending_recursive_dict_update(settings, settings_user)
 
-        try:
-            return Settings(settings)
-        except AttributeError as e:
-            raise ConanException("Invalid settings.yml format: {}".format(e))
+        return Settings(settings)
 
     def initialize_settings(self):
         # TODO: This is called by ConfigAPI.init(), maybe move everything there?
         if not os.path.exists(self.settings_path):
             settings_yml = default_settings_yml
             save(self.settings_path, settings_yml)
             save(self.settings_path + ".orig", settings_yml)  # stores a copy, to check migrations
```

### Comparing `conan-2.0.4/conans/client/cache/editable.py` & `conan-2.0.5/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/cache/remote_registry.py` & `conan-2.0.5/conans/client/cache/remote_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,105 +1,121 @@
 import json
 import os
 from urllib.parse import urlparse
 
 from conan.api.model import Remote
 from conan.api.output import ConanOutput
-from conans.errors import ConanException, NoRemoteAvailable
+from conans.errors import ConanException
 from conans.util.files import load, save
 
 CONAN_CENTER_REMOTE_NAME = "conancenter"
 
 
-class _Remotes(object):
+class _Remotes:
     """Class to manage an ordered list of Remote objects, performing validations
     and updating the remotes. Used by RemoteRegistry only! """
 
     def __init__(self):
-        self._remotes = []
+        self._remotes = {}
 
     def __bool__(self):
         return bool(self._remotes)
 
-    def rename(self, remote, new_remote_name):
-        if self.get_by_name(new_remote_name):
+    def __getitem__(self, remote_name):
+        try:
+            return self._remotes[remote_name]
+        except KeyError:
+            raise ConanException(f"Remote '{remote_name}' doesn't exist")
+
+    @staticmethod
+    def load(filename):
+        text = load(filename)
+        result = _Remotes()
+        data = json.loads(text)
+        for r in data.get("remotes", []):
+            disabled = r.get("disabled", False)
+            # TODO: Remote.serialize/deserialize
+            remote = Remote(r["name"], r["url"], r["verify_ssl"], disabled)
+            result._remotes[r["name"]] = remote
+        return result
+
+    def dumps(self):
+        remote_list = []
+        for r in self._remotes.values():
+            remote = {"name": r.name, "url": r.url, "verify_ssl": r.verify_ssl}
+            if r.disabled:
+                remote["disabled"] = True
+            remote_list.append(remote)
+        ret = {"remotes": remote_list}
+        return json.dumps(ret, indent=True)
+
+    def rename(self, remote_name, new_remote_name):
+        if new_remote_name in self._remotes:
             raise ConanException("Remote '%s' already exists" % new_remote_name)
 
-        r = self.get_by_name(remote.name)
+        r = self[remote_name]
         r._name = new_remote_name
-        remote._name = new_remote_name
-
-    @property
-    def default(self):
-        ret = self._remotes[0]
-        if not ret:
-            raise NoRemoteAvailable("No default remote defined")
-        return ret
+        # Keep the remotes order
+        self._remotes = {r.name: r for r in self._remotes.values()}
 
     def remove(self, remote_name):
-        r = self.get_by_name(remote_name)
-        if r is None:
-            raise ConanException("The specified remote doesn't exist")
-        index = self._remotes.index(r)
-        return self._remotes.pop(index)
+        try:
+            self._remotes.pop(remote_name)
+        except KeyError:
+            raise ConanException(f"Remote '{remote_name}' doesn't exist")
 
     def add(self, new_remote: Remote, index=None, force=False):
         assert isinstance(new_remote, Remote)
-        current = self.get_by_name(new_remote.name)
+        current = self._remotes.get(new_remote.name)
         if current:  # same name remote existing!
             if not force:
                 raise ConanException(f"Remote '{new_remote.name}' already exists in remotes "
                                      "(use --force to continue)")
-
             ConanOutput().warning(f"Remote '{new_remote.name}' already exists in remotes")
             if current.url != new_remote.url:
                 ConanOutput().warning("Updating existing remote with new url")
-            current_index = self._remotes.index(current)
-            self._remotes.remove(current)
-            index = index or current_index
-            self._remotes.insert(index, new_remote)
-            return
 
+        self._check_urls(new_remote.url, force, current)
+        if index is None:
+            self._remotes[new_remote.name] = new_remote
+        else:
+            self._remotes.pop(new_remote.name, None)
+            remotes = list(self._remotes.values())
+            remotes.insert(index, new_remote)
+            self._remotes = {r.name: r for r in remotes}
+
+    def _check_urls(self, url, force, current):
         # The remote name doesn't exist
-        for r in self._remotes:
-            if r.url == new_remote.url:
+        for r in self._remotes.values():
+            if r is not current and r.url == url:
                 msg = f"Remote url already existing in remote '{r.name}'. " \
                       f"Having different remotes with same URL is not recommended."
                 if not force:
                     raise ConanException(msg + " Use '--force' to override.")
                 else:
-                    ConanOutput().warning(msg + " Adding duplicated remote because '--force'.")
-        if index:
-            self._remotes.insert(index, new_remote)
-        else:
-            self._remotes.append(new_remote)
+                    ConanOutput().warning(msg + " Adding duplicated remote url because '--force'.")
 
-    def update(self, remote: Remote):
-        assert isinstance(remote, Remote)
-        current = self.get_by_name(remote.name)
-        if not current:
-            raise ConanException("The remote '{}' doesn't exist".format(remote.name))
-
-        index = self._remotes.index(current)
-        self._remotes.remove(current)
-        self._remotes.insert(index, remote)
-
-    def move(self, remote: Remote, new_index: int):
-        assert isinstance(remote, Remote)
-        self.remove(remote.name)
-        self._remotes.insert(new_index, remote)
-
-    def get_by_name(self, name):
-        for r in self._remotes:
-            if r.name == name:
-                return r
-        return None
+    def update(self, remote_name, url=None, secure=None, disabled=None, index=None, force=False):
+        remote = self[remote_name]
+        if url is not None:
+            self._check_urls(url, force, remote)
+            remote.url = url
+        if secure is not None:
+            remote.verify_ssl = secure
+        if disabled is not None:
+            remote.disabled = disabled
+
+        if index is not None:
+            self._remotes.pop(remote.name, None)
+            remotes = list(self._remotes.values())
+            remotes.insert(index, remote)
+            self._remotes = {r.name: r for r in remotes}
 
     def items(self):
-        return self._remotes
+        return list(self._remotes.values())
 
 
 class RemoteRegistry(object):
     """Store remotes in disk and modify remotes for the 'conan remote' command.
     It never returns an _Remotes object, only Remote model"""
 
     def __init__(self, cache):
@@ -124,76 +140,43 @@
             remotes = _Remotes()
             remote = Remote(CONAN_CENTER_REMOTE_NAME, "https://center.conan.io", True, False)
             remotes.add(remote)
             self.save_remotes(remotes)
 
     def _load_remotes(self):
         self.initialize_remotes()
-        content = load(self._filename)
-        result = _Remotes()
-        data = json.loads(content)
-        for r in data.get("remotes", []):
-            disabled = r.get("disabled", False)
-            remote = Remote(r["name"], r["url"], r["verify_ssl"], disabled)
-            result._remotes.append(remote)
-        return result
-
-    @staticmethod
-    def _dumps_json(remotes):
-        ret = {"remotes": []}
-        for r in remotes.items():
-            remote = {"name": r.name, "url": r.url, "verify_ssl": r.verify_ssl}
-            if r.disabled:
-                remote["disabled"] = True
-            ret["remotes"].append(remote)
-        return json.dumps(ret, indent=True)
+        return _Remotes.load(self._filename)
 
     def list(self):
         return self._load_remotes().items()
 
-    @property
-    def default(self):
-        return self.list()[0]
-
     def read(self, remote_name):
         remotes = self._load_remotes()
-        ret = remotes.get_by_name(remote_name)
-        if not ret:
-            raise ConanException("Remote '%s' not found in remotes" % remote_name)
+        ret = remotes[remote_name]
         return ret
 
-    def get_remote_index(self, remote: Remote):
-        try:
-            return self.list().index(remote)
-        except ValueError:
-            raise ConanException("No remote: '{}' found".format(remote.name))
-
-    def add(self, remote: Remote, force=False):
+    def add(self, remote: Remote, force=False, index=None):
         self._validate_url(remote.url)
         remotes = self._load_remotes()
-        remotes.add(remote, force=force)
+        remotes.add(remote, force=force, index=index)
         self.save_remotes(remotes)
 
     def remove(self, remote_name):
         assert isinstance(remote_name, str)
         remotes = self._load_remotes()
         remotes.remove(remote_name)
         self.save_remotes(remotes)
 
-    def update(self, remote):
-        self._validate_url(remote.url)
-        remotes = self._load_remotes()
-        remotes.update(remote)
-        self.save_remotes(remotes)
-
-    def move(self, remote, index):
+    def update(self, remote_name, url, secure, disabled, index):
+        if url is not None:
+            self._validate_url(url)
         remotes = self._load_remotes()
-        remotes.move(remote, new_index=index)
+        remotes.update(remote_name, url, secure, disabled, index)
         self.save_remotes(remotes)
 
     def rename(self, remote, new_name):
         remotes = self._load_remotes()
         remotes.rename(remote, new_name)
         self.save_remotes(remotes)
 
     def save_remotes(self, remotes):
-        save(self._filename, self._dumps_json(remotes))
+        save(self._filename, remotes.dumps())
```

### Comparing `conan-2.0.4/conans/client/cmd/export.py` & `conan-2.0.5/conans/client/cmd/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,36 +80,35 @@
             set_dirty(source_folder)
 
     scoped_output.success(f"Exported: {ref.repr_humantime()}")
     return ref, conanfile
 
 
 def _calc_revision(scoped_output, path, manifest, revision_mode):
-    if revision_mode not in ["scm", "hash"]:
+    if revision_mode not in ["scm", "scm_folder", "hash"]:
         raise ConanException("Revision mode should be one of 'hash' (default) or 'scm'")
 
     # Use the proper approach depending on 'revision_mode'
     if revision_mode == "hash":
         revision = manifest.summary_hash
     else:
         try:
             with chdir(path):
-                rev_detected = check_output_runner('git rev-list HEAD -n 1 --full-history').strip()
+                f = '-- "."' if revision_mode == "scm_folder" else ""
+                revision = check_output_runner(f'git rev-list HEAD -n 1 --full-history {f}').strip()
         except Exception as exc:
             error_msg = "Cannot detect revision using '{}' mode from repository at " \
                         "'{}'".format(revision_mode, path)
             raise ConanException("{}: {}".format(error_msg, exc))
 
         with chdir(path):
             if bool(check_output_runner('git status -s').strip()):
                 raise ConanException("Can't have a dirty repository using revision_mode='scm' and doing"
                                      " 'conan export', please commit the changes and run again.")
 
-        revision = rev_detected
-
         scoped_output.info("Using git commit as the recipe revision: %s" % revision)
 
     return revision
 
 
 def _classify_patterns(patterns):
     patterns = patterns or []
```

### Comparing `conan-2.0.4/conans/client/cmd/uploader.py` & `conan-2.0.5/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/cmd/user.py` & `conan-2.0.5/conans/client/cmd/user.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conanfile/build.py` & `conan-2.0.5/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conanfile/configure.py` & `conan-2.0.5/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conanfile/package.py` & `conan-2.0.5/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conf/__init__.py` & `conan-2.0.5/conans/client/conf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # will destroy your changes.
 os:
     Windows:
         subsystem: [null, cygwin, msys, msys2, wsl]
     WindowsStore:
         version: ["8.1", "10.0"]
     WindowsCE:
-        platform: ANY
+        platform: [ANY]
         version: ["5.0", "6.0", "7.0", "8.0"]
     Linux:
     iOS:
         version: &ios_version
                    ["7.0", "7.1", "8.0", "8.1", "8.2", "8.3", "9.0", "9.1", "9.2", "9.3", "10.0", "10.1", "10.2", "10.3",
                     "11.0", "11.1", "11.2", "11.3", "11.4", "12.0", "12.1", "12.2", "12.3", "12.4",
                     "13.0", "13.1", "13.2", "13.3", "13.4", "13.5", "13.6", "13.7",
@@ -70,15 +70,16 @@
                     "5", "5.1", "5.2", "5.3", "5.4", "5.5",
                     "6", "6.1", "6.2", "6.3", "6.4", "6.5",
                     "7", "7.1", "7.2", "7.3", "7.4", "7.5",
                     "8", "8.1", "8.2", "8.3", "8.4", "8.5",
                     "9", "9.1", "9.2", "9.3", "9.4", "9.5",
                     "10", "10.1", "10.2", "10.3", "10.4",
                     "11", "11.1", "11.2", "11.3",
-                    "12", "12.1", "12.2"]
+                    "12", "12.1", "12.2", "12.3",
+                    "13", "13.1"]
         libcxx: [libstdc++, libstdc++11]
         threads: [null, posix, win32]  # Windows MinGW
         exception: [null, dwarf2, sjlj, seh]  # Windows MinGW
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
     msvc:
         version: [170, 180, 190, 191, 192, 193]
         update: [null, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
@@ -100,15 +101,15 @@
         libcxx: [libstdc++, libc++]
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
     intel-cc:
         version: ["2021.1", "2021.2", "2021.3"]
         update: [null, ANY]
         mode: ["icx", "classic", "dpcpp"]
         libcxx: [null, libstdc++, libstdc++11, libc++]
-        cppstd: [null, 98, gnu98, 03, gnu03, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
+        cppstd: [null, 98, gnu98, "03", gnu03, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
         runtime: [null, static, dynamic]
         runtime_type: [null, Debug, Release]
     qcc:
         version: ["4.4", "5.4", "8.3"]
         libcxx: [cxx, gpp, cpp, cpp-ne, accp, acpp-ne, ecpp, ecpp-ne]
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17]
     mcst-lcc:
@@ -124,8 +125,8 @@
     return default_settings_yml
 
 
 def migrate_settings_file(cache):
     from conans.client.migrations import update_file
 
     settings_path = cache.settings_path
-    update_file(settings_path, get_default_settings_yml())
+    update_file(settings_path, default_settings_yml)
```

### Comparing `conan-2.0.4/conans/client/conf/config_installer.py` & `conan-2.0.5/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conf/detect.py` & `conan-2.0.5/conans/client/conf/detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,27 +330,27 @@
     elif "e2k" in machine:
         return _get_e2k_architecture()
 
     return None
 
 
 def _detect_os_arch(result):
-    from conans.client.conf import get_default_settings_yml
+    from conans.client.conf import default_settings_yml
     from conans.model.settings import Settings
 
     the_os = platform.system()
     if the_os == "Darwin":
         the_os = "Macos"
     result.append(("os", the_os))
 
     arch = _detected_architecture()
 
     if arch:
         if arch.startswith('arm'):
-            settings = Settings.loads(get_default_settings_yml())
+            settings = Settings.loads(default_settings_yml)
             defined_architectures = settings.arch.values_range
             defined_arm_architectures = [v for v in defined_architectures if v.startswith("arm")]
 
             for a in defined_arm_architectures:
                 if arch.startswith(a):
                     arch = a
                     break
```

### Comparing `conan-2.0.4/conans/client/conf/detect_vs.py` & `conan-2.0.5/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/conf/required_version.py` & `conan-2.0.5/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/downloaders/caching_file_downloader.py` & `conan-2.0.5/conans/client/downloaders/caching_file_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,19 @@
         with download_cache.lock(sha256):
             remove_if_dirty(cached_path)
 
             if os.path.exists(cached_path):
                 self._output.info(f"Source {urls} retrieved from local download cache")
             else:
                 with set_dirty_context_manager(cached_path):
+                    if None in backups_urls:
+                        raise ConanException("Trying to download sources from None backup remote."
+                                             f" Remotes were: {backups_urls}")
                     for backup_url in backups_urls:
+
                         is_last = backup_url is backups_urls[-1]
                         if backup_url == "origin":  # recipe defined URLs
                             if self._origin_download(urls, cached_path, retry, retry_wait,
                                                      verify_ssl, auth, headers, md5, sha1, sha256,
                                                      is_last):
                                 break
                         else:
```

### Comparing `conan-2.0.4/conans/client/downloaders/download_cache.py` & `conan-2.0.5/conans/client/downloaders/download_cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,20 +41,29 @@
             thread_lock.acquire()
             try:
                 yield
             finally:
                 thread_lock.release()
 
     def get_backup_sources_files_to_upload(self, package_list):
-        """ from a package_list of packages to upload, collect from the backup-sources ccache
+        """ from a package_list of packages to upload, collect from the backup-sources cache
         the matching references to upload those backups too
         """
+        def should_upload_sources(package):
+            return any(prev["upload"] for prev in package["revisions"].values())
+
         files_to_upload = []
         path_backups = os.path.join(self._path, self._SOURCE_BACKUP)
-        all_refs = {str(k) for k, v in package_list.refs() if v.get("upload")}
+
+        if not os.path.exists(path_backups):
+            return []
+
+        all_refs = {str(k) for k, ref in package_list.refs()
+                    if ref.get("upload") or any(should_upload_sources(p)
+                                                for p in ref["packages"].values())}
         for f in os.listdir(path_backups):
             if f.endswith(".json"):
                 f = os.path.join(path_backups, f)
                 content = json.loads(load(f))
                 refs = content["references"]
                 # unknown entries are not uploaded at this moment, the flow is not expected.
                 if any(ref in all_refs for ref in refs):
@@ -79,8 +88,11 @@
             # So best we can do is to set this as unknown
             summary_key = "unknown"
 
         if not isinstance(urls, (list, tuple)):
             urls = [urls]
         existing_urls = summary["references"].setdefault(summary_key, [])
         existing_urls.extend(url for url in urls if url not in existing_urls)
+        conanfile.output.verbose(f"Updating ${summary_path} summary file")
+        summary_dump = json.dumps(summary)
+        conanfile.output.debug(f"New summary: ${summary_dump}")
         save(summary_path, json.dumps(summary))
```

### Comparing `conan-2.0.4/conans/client/downloaders/file_downloader.py` & `conan-2.0.5/conans/client/downloaders/file_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 total_size = response.headers.get('Content-Length') or len(response.content)
                 return int(total_size)
 
         try:
             total_length = get_total_length()
             if total_length > 100000:
                 action = "Downloading" if range_start == 0 else "Continuing download of"
-                description = "{} {}".format(action, os.path.basename(file_path))
+                description = f"${action} {os.path.basename(file_path)} from {url}"
                 self._output.info(description)
 
             chunk_size = 1024 * 100
             total_downloaded_size = range_start
             mode = "ab" if range_start else "wb"
             with open(file_path, mode) as file_handler:
                 for chunk in response.iter_content(chunk_size):
```

### Comparing `conan-2.0.4/conans/client/generators/__init__.py` & `conan-2.0.5/conans/client/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import os
 import traceback
 import importlib
 
 from conans.client.subsystems import deduce_subsystem, subsystem_path
 from conans.errors import ConanException, conanfile_exception_formatter
 from conans.util.files import save, mkdir, chdir
@@ -41,30 +42,51 @@
                              f"Could not find module {generator_class}") from e
     except AttributeError as e:
         raise ConanException("Internal Conan error: "
                              f"Could not find name {generator_name} "
                              f"inside module {generator_class}") from e
 
 
-def write_generators(conanfile, hook_manager):
+def load_cache_generators(path):
+    from conans.client.loader import load_python_file
+    result = {}  # Name of the generator: Class
+    if not os.path.isdir(path):
+        return result
+    for f in os.listdir(path):
+        if not f.endswith(".py") or f.startswith("_"):
+            continue
+        full_path = os.path.join(path, f)
+        mod, _ = load_python_file(full_path)
+        for name, value in inspect.getmembers(mod):
+            if inspect.isclass(value) and not name.startswith("_"):
+                result = {name: value}
+    return result
+
+
+def write_generators(conanfile, app):
     new_gen_folder = conanfile.generators_folder
     _receive_conf(conanfile)
 
+    hook_manager = app.hook_manager
+    cache = app.cache
+    # TODO: Optimize this, so the global generators are not loaded every call to write_generators
+    global_generators = load_cache_generators(cache.custom_generators_path)
     hook_manager.execute("pre_generate", conanfile=conanfile)
 
     if conanfile.generators:
         conanfile.output.highlight(f"Writing generators to {new_gen_folder}")
     # generators check that they are not present in the generators field,
     # to avoid duplicates between the generators attribute and the generate() method
     # They would raise an exception here if we don't invalidate the field while we call them
     old_generators = set(conanfile.generators)
     conanfile.generators = []
     try:
         for generator_name in old_generators:
-            generator_class = _get_generator_class(generator_name)
+            global_generator = global_generators.get(generator_name)
+            generator_class = global_generator or _get_generator_class(generator_name)
             if generator_class:
                 try:
                     generator = generator_class(conanfile)
                     mkdir(new_gen_folder)
                     conanfile.output.info(f"Generator '{generator_name}' calling 'generate()'")
                     with chdir(new_gen_folder):
                         generator.generate()
@@ -117,15 +139,15 @@
 
 
 def _generate_aggregated_env(conanfile):
 
     def deactivates(filenames):
         # FIXME: Probably the order needs to be reversed
         result = []
-        for s in filenames:
+        for s in reversed(filenames):
             folder, f = os.path.split(s)
             result.append(os.path.join(folder, "deactivate_{}".format(f)))
         return result
 
     generated = []
     for group, env_scripts in conanfile.env_scripts.items():
         subsystem = deduce_subsystem(conanfile, group)
```

### Comparing `conan-2.0.4/conans/client/graph/build_mode.py` & `conan-2.0.5/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/compatibility.py` & `conan-2.0.5/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/compute_pid.py` & `conan-2.0.5/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/graph.py` & `conan-2.0.5/conans/client/graph/graph.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import OrderedDict
 
 from conans.model.package_ref import PkgReference
+from conans.model.recipe_ref import RecipeReference
 
 RECIPE_DOWNLOADED = "Downloaded"
 RECIPE_INCACHE = "Cache"  # The previously installed recipe in cache is being used
 RECIPE_UPDATED = "Updated"
 RECIPE_INCACHE_DATE_UPDATED = "Cache (Updated date)"
 RECIPE_NEWER = "Newer"  # The local recipe is  modified and newer timestamp than server
 RECIPE_NOT_IN_REMOTE = "Not in remote"
@@ -214,36 +215,113 @@
         result["package_id"] = self.package_id
         result["prev"] = self.prev
         from conans.client.installer import build_id
         result["build_id"] = build_id(self.conanfile)
         result["binary"] = self.binary
         # TODO: This doesn't match the model, check it
         result["invalid_build"] = self.cant_build
+        result["info_invalid"] = getattr(getattr(self.conanfile, "info", None), "invalid", None)
         # Adding the conanfile information: settings, options, etc
         result.update(self.conanfile.serialize())
         result["context"] = self.context
         result["test"] = self.test
         result["requires"] = {n.id: n.ref.repr_notime() for n in self.neighbors()}
         return result
 
+    def overrides(self):
+
+        def transitive_subgraph():
+            result = set()
+            opened = {self}
+            while opened:
+                new_opened = set()
+                for o in opened:
+                    result.add(o)
+                    new_opened.update(set(o.neighbors()).difference(result))
+                opened = new_opened
+
+            return result
+
+        nodes = transitive_subgraph()
+        return Overrides.create(nodes)
+
 
 class Edge(object):
     def __init__(self, src, dst, require):
         self.src = src
         self.dst = dst
         self.require = require
 
 
+class Overrides:
+    def __init__(self):
+        self._overrides = {}  # {require_ref: {override_ref1, override_ref2}}
+
+    def __bool__(self):
+        return bool(self._overrides)
+
+    def __repr__(self):
+        return repr(self.serialize())
+
+    @staticmethod
+    def create(nodes):
+        overrides = {}
+        for n in nodes:
+            for r in n.conanfile.requires.values():
+                if r.override:
+                    continue
+                if r.overriden_ref and not r.force:
+                    overrides.setdefault(r.overriden_ref, set()).add(r.override_ref)
+                else:
+                    overrides.setdefault(r.ref, set()).add(None)
+
+        # reduce, eliminate those overrides definitions that only override to None, that is, not
+        # really an override
+        result = Overrides()
+        for require, override_info in overrides.items():
+            if len(override_info) != 1 or None not in override_info:
+                result._overrides[require] = override_info
+        return result
+
+    def get(self, require):
+        return self._overrides.get(require)
+
+    def update(self, other):
+        """
+        @type other: Overrides
+        """
+        for require, override_info in other._overrides.items():
+            self._overrides.setdefault(require, set()).update(override_info)
+
+    def items(self):
+        return self._overrides.items()
+
+    def serialize(self):
+        return {k.repr_notime(): [e.repr_notime() if e else None for e in v]
+                for k, v in self._overrides.items()}
+
+    @staticmethod
+    def deserialize(data):
+        result = Overrides()
+        result._overrides = {RecipeReference.loads(k):
+                             set([RecipeReference.loads(e) if e else None for e in v])
+                             for k, v in data.items()}
+        return result
+
+
 class DepsGraph(object):
     def __init__(self):
         self.nodes = []
         self.aliased = {}
         self.resolved_ranges = {}
         self.error = False
 
+    def overrides(self):
+        return Overrides.create(self.nodes)
+
     def __repr__(self):
         return "\n".join((repr(n) for n in self.nodes))
 
     @property
     def root(self):
         return self.nodes[0] if self.nodes else None
```

### Comparing `conan-2.0.4/conans/client/graph/graph_binaries.py` & `conan-2.0.5/conans/client/graph/graph_binaries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from conan.api.output import ConanOutput
 from conans.client.graph.build_mode import BuildMode
 from conans.client.graph.compatibility import BinaryCompatibility
 from conans.client.graph.compute_pid import compute_package_id
 from conans.client.graph.graph import (BINARY_BUILD, BINARY_CACHE, BINARY_DOWNLOAD, BINARY_MISSING,
                                        BINARY_UPDATE, RECIPE_EDITABLE, BINARY_EDITABLE,
                                        RECIPE_CONSUMER, RECIPE_VIRTUAL, BINARY_SKIP,
                                        BINARY_INVALID, BINARY_EDITABLE_BUILD, RECIPE_SYSTEM_TOOL,
@@ -19,22 +20,17 @@
         self._evaluated = {}  # {pref: [nodes]}
         self._compatibility = BinaryCompatibility(self._cache)
 
     @staticmethod
     def _evaluate_build(node, build_mode):
         ref, conanfile = node.ref, node.conanfile
         with_deps_to_build = False
-        # For cascade mode, we need to check also the "modified" status of the lockfile if exists
-        # modified nodes have already been built, so they shouldn't be built again
+        # check dependencies, if they are being built, "cascade" will try to build this one too
         if build_mode.cascade:
-            for dep in node.dependencies:
-                dep_node = dep.dst
-                if dep_node.binary == BINARY_BUILD:
-                    with_deps_to_build = True
-                    break
+            with_deps_to_build = any(dep.dst.binary == BINARY_BUILD for dep in node.dependencies)
         if build_mode.forced(conanfile, ref, with_deps_to_build):
             node.should_build = True
             conanfile.output.info('Forced build from source')
             node.binary = BINARY_BUILD if not node.cant_build else BINARY_INVALID
             node.prev = None
             return True
 
@@ -135,15 +131,15 @@
 
     def _evaluate_node(self, node, build_mode):
         assert node.binary is None, "Node.binary should be None"
         assert node.package_id is not None, "Node.package_id shouldn't be None"
         assert node.prev is None, "Node.prev should be None"
 
         self._process_node(node, build_mode)
-        if node.binary in (BINARY_MISSING,) \
+        if node.binary == BINARY_MISSING \
                 and not build_mode.should_build_missing(node.conanfile) and not node.should_build:
             self._process_compatible_packages(node)
 
         if node.binary == BINARY_MISSING and build_mode.allowed(node.conanfile):
             node.should_build = True
             node.binary = BINARY_BUILD if not node.cant_build else BINARY_INVALID
 
@@ -183,15 +179,24 @@
             cache_latest_prev = self._cache.get_latest_package_reference(node.pref)
             if cache_latest_prev is None:
                 break
             package_layout = self._cache.pkg_layout(cache_latest_prev)
             if not self._evaluate_clean_pkg_folder_dirty(node, package_layout):
                 break
 
-        if cache_latest_prev is None:  # This binary does NOT exist in the cache
+        if node.conanfile.upload_policy == "skip":
+            if cache_latest_prev:
+                node.binary = BINARY_CACHE
+                node.prev = cache_latest_prev.revision
+            elif build_mode.allowed(node.conanfile):
+                node.should_build = True
+                node.binary = BINARY_BUILD
+            else:
+                node.binary = BINARY_MISSING
+        elif cache_latest_prev is None:  # This binary does NOT exist in the cache
             self._evaluate_download(node)
         else:  # This binary already exists in the cache, maybe can be updated
             self._evaluate_in_cache(cache_latest_prev, node)
 
         # The INVALID should only prevail if a compatible package, due to removal of
         # settings in package_id() was not found
         if node.binary in (BINARY_MISSING, BINARY_BUILD):
@@ -304,14 +309,18 @@
         self._update = update  # TODO: Dirty, fix it
         test_package = deps_graph.root.conanfile.tested_reference_str is not None
         if test_package:
             main_mode = BuildMode(["never"])
             test_mode = BuildMode(build_mode)
         else:
             main_mode = test_mode = BuildMode(build_mode)
+        if main_mode.cascade:
+            ConanOutput().warning("Using build-mode 'cascade' is generally inefficient and it "
+                                  "shouldn't be used. Use 'package_id' and 'package_id_modes' for"
+                                  "more efficient re-builds")
         for node in deps_graph.ordered_iterate():
             build_mode = test_mode if node.test_package else main_mode
             if node.recipe in (RECIPE_CONSUMER, RECIPE_VIRTUAL):
                 if node.path is not None and node.path.endswith(".py"):
                     # For .py we keep evaluating the package_id, validate(), etc
                     self._evaluate_package_id(node)
                 elif node.path is not None and node.path.endswith(".txt"):
```

### Comparing `conan-2.0.4/conans/client/graph/graph_builder.py` & `conan-2.0.5/conans/client/graph/graph_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,16 @@
             # print("  Existing previous requirements from ", base_previous, "=>", prev_require)
 
             if prev_require is None:
                 raise GraphLoopError(node, require, prev_node)
 
             prev_ref = prev_node.ref if prev_node else prev_require.ref
             if prev_require.force or prev_require.override:  # override
+                require.overriden_ref = require.ref  # Store that the require has been overriden
+                require.override_ref = prev_ref
                 require.ref = prev_ref
             else:
                 self._conflicting_version(require, node, prev_require, prev_node,
                                           prev_ref, base_previous, self._resolve_prereleases)
 
         if prev_node is None:
             # new node, must be added and expanded (node -> new_node)
@@ -153,29 +155,26 @@
                     if str(tool_require) == str(ref):  # FIXME: Ugly str comparison
                         continue  # avoid self-loop of build-requires in build context
                     # FIXME: converting back to string?
                     node.conanfile.requires.tool_require(str(tool_require),
                                                          raise_if_duplicated=False)
 
     def _initialize_requires(self, node, graph, graph_lock):
-        # Introduce the current requires to define overrides
-        # This is the first pass over one recipe requires
-        if graph_lock is not None:
-            for require in node.conanfile.requires.values():
-                graph_lock.resolve_locked(node, require, self._resolve_prereleases)
-
         for require in node.conanfile.requires.values():
-            self._resolve_alias(node, require, graph)
+            alias = require.alias  # alias needs to be processed this early
+            if alias is not None:
+                resolved = False
+                if graph_lock is not None:
+                    resolved = graph_lock.replace_alias(require, alias)
+                # if partial, we might still need to resolve the alias
+                if not resolved:
+                    self._resolve_alias(node, require, alias, graph)
             node.transitive_deps[require] = TransitiveRequirement(require, node=None)
 
-    def _resolve_alias(self, node, require, graph):
-        alias = require.alias
-        if alias is None:
-            return
-
+    def _resolve_alias(self, node, require, alias, graph):
         # First try cached
         cached = graph.aliased.get(alias)
         if cached is not None:
             while True:
                 new_cached = graph.aliased.get(cached)
                 if new_cached is None:
                     break
@@ -230,14 +229,29 @@
                     elif require.ref.version == d.version:
                         if d.revision is None or require.ref.revision is None or \
                                 d.revision == require.ref.revision:
                             require.ref.revision = d.revision
                             return d, ConanFile(str(d)), RECIPE_SYSTEM_TOOL, None
 
     def _create_new_node(self, node, require, graph, profile_host, profile_build, graph_lock):
+        if require.ref.version == "<host_version>":
+            if not require.build or require.visible:
+                raise ConanException(f"{node.ref} require '{require.ref}': 'host_version' can only "
+                                     "be used for non-visible tool_requires")
+            req = Requirement(require.ref, headers=True, libs=True, visible=True)
+            transitive = node.transitive_deps.get(req)
+            if transitive is None:
+                raise ConanException(f"{node.ref} require '{require.ref}': didn't find a matching "
+                                     "host dependency")
+            require.ref.version = transitive.require.ref.version
+
+        if graph_lock is not None:
+            # Here is when the ranges and revisions are resolved
+            graph_lock.resolve_locked(node, require, self._resolve_prereleases)
+
         resolved = self._resolved_system_tool(node, require, profile_build, profile_host,
                                               self._resolve_prereleases)
 
         if resolved is None:
             try:
                 # TODO: If it is locked not resolve range
                 # TODO: This range-resolve might resolve in a given remote or cache
```

### Comparing `conan-2.0.4/conans/client/graph/graph_error.py` & `conan-2.0.5/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/install_graph.py` & `conan-2.0.5/conans/client/graph/install_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import textwrap
 
 from conan.api.output import ConanOutput
 from conans.client.graph.graph import RECIPE_CONSUMER, RECIPE_VIRTUAL, BINARY_SKIP, \
-    BINARY_MISSING, BINARY_INVALID
+    BINARY_MISSING, BINARY_INVALID, Overrides, BINARY_BUILD
 from conans.errors import ConanInvalidConfiguration, ConanException
 from conans.model.recipe_ref import RecipeReference
 from conans.util.files import load
 
 
 class _InstallPackageReference:
     """ Represents a single, unique PackageReference to be downloaded, built, etc.
@@ -25,54 +25,73 @@
         # be able to reproduce, typically host preferrably
         self.options = []  # to be able to fire a build, the options will be necessary
         self.filenames = []  # The build_order.json filenames e.g. "windows_build_order"
         # If some package, like ICU, requires itself, built for the "build" context architecture
         # to cross compile, there will be a dependency from the current "self" (host context)
         # to that "build" package_id.
         self.depends = []  # List of package_ids of dependencies to other binaries of the same ref
+        self.overrides = Overrides()
+        self.ref = None
 
     @staticmethod
     def create(node):
         result = _InstallPackageReference()
+        result.ref = node.ref
         result.package_id = node.pref.package_id
         result.prev = node.pref.revision
         result.binary = node.binary
         result.context = node.context
         # self_options are the minimum to reproduce state
         result.options = node.conanfile.self_options.dumps().splitlines()
         result.nodes.append(node)
+        result.overrides = node.overrides()
         return result
 
     def add(self, node):
         assert self.package_id == node.package_id
         assert self.binary == node.binary
         assert self.prev == node.prev
         # The context might vary, but if same package_id, all fine
         # assert self.context == node.context
         self.nodes.append(node)
 
+    def _build_args(self):
+        if self.binary != BINARY_BUILD:
+            return None
+        cmd = f"--require={self.ref}" if self.context == "host" else f"--tool-require={self.ref}"
+        cmd += f" --build={self.ref}"
+        if self.options:
+            cmd += " " + " ".join(f"-o {o}" for o in self.options)
+        if self.overrides:
+            cmd += f' --lockfile-overrides="{self.overrides}"'
+        return cmd
+
     def serialize(self):
         return {"package_id": self.package_id,
                 "prev": self.prev,
                 "context": self.context,
                 "binary": self.binary,
                 "options": self.options,
                 "filenames": self.filenames,
-                "depends": self.depends}
+                "depends": self.depends,
+                "overrides": self.overrides.serialize(),
+                "build_args": self._build_args()}
 
     @staticmethod
-    def deserialize(data, filename):
+    def deserialize(data, filename, ref):
         result = _InstallPackageReference()
+        result.ref = ref
         result.package_id = data["package_id"]
         result.prev = data["prev"]
         result.binary = data["binary"]
         result.context = data["context"]
         result.options = data["options"]
         result.filenames = data["filenames"] or [filename]
         result.depends = data["depends"]
+        result.overrides = Overrides.deserialize(data["overrides"])
         return result
 
 
 class _InstallRecipeReference:
     """ represents a single, unique Recipe reference (including revision, must have it) containing
     all the _InstallPackageReference that belongs to this RecipeReference. This approach is
     oriented towards a user-intuitive grouping specially in CI, in which all binary variants for the
@@ -150,15 +169,15 @@
     def deserialize(data, filename):
         result = _InstallRecipeReference()
         result.ref = RecipeReference.loads(data["ref"])
         for d in data["depends"]:
             result.depends.append(RecipeReference.loads(d))
         for level in data["packages"]:
             for p in level:
-                install_node = _InstallPackageReference.deserialize(p, filename)
+                install_node = _InstallPackageReference.deserialize(p, filename, result.ref)
                 result.packages[install_node.package_id] = install_node
         return result
 
 
 class InstallGraph:
     """ A graph containing the package references in order to be built/downloaded
     """
```

### Comparing `conan-2.0.4/conans/client/graph/profile_node_definer.py` & `conan-2.0.5/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/provides.py` & `conan-2.0.5/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/proxy.py` & `conan-2.0.5/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/graph/python_requires.py` & `conan-2.0.5/conans/client/graph/python_requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 
     def _resolve_ref(self, requirement, graph_lock, remotes, update):
         if requirement.alias:
             raise ConanException("python-requires 'alias' are not supported in Conan 2.0. "
                                  "Please use version ranges instead")
         if graph_lock:
             graph_lock.resolve_locked_pyrequires(requirement)
-        else:
-            self._range_resolver.resolve(requirement, "py_require", remotes, update)
+        # If the lock hasn't resolved the range, and it hasn't failed (it is partial), resolve it
+        self._range_resolver.resolve(requirement, "py_require", remotes, update)
         ref = requirement.ref
         return ref
 
     def _load_pyreq_conanfile(self, loader, graph_lock, ref, remotes, update, check_update):
         try:
             recipe = self._proxy.get_recipe(ref, remotes, update, check_update)
         except ConanException as e:
```

### Comparing `conan-2.0.4/conans/client/graph/range_resolver.py` & `conan-2.0.5/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/hook_manager.py` & `conan-2.0.5/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/installer.py` & `conan-2.0.5/conans/client/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             except Exception as e:
                 msg = str(e)
                 if "206" in msg:  # System error shutil.Error 206: Filename or extension too long
                     msg += "\nUse short_paths=True if paths too long"
                 raise ConanException("%s\nError copying sources to build folder" % msg)
 
     def _build(self, conanfile, pref):
-        write_generators(conanfile, self._hook_manager)
+        write_generators(conanfile, self._app)
 
         try:
             run_build_method(conanfile, self._hook_manager)
             conanfile.output.success("Package '%s' built" % pref.package_id)
             conanfile.output.info("Build folder %s" % conanfile.build_folder)
         except Exception as exc:
             conanfile.output.error("\nPackage '%s' build failed" % pref.package_id)
@@ -347,15 +347,15 @@
 
         # TODO: Check, this assumes the folder is always the conanfile one
         base_path = os.path.dirname(conanfile_path)
         conanfile.folders.set_base_folders(base_path, output_folder)
         output = conanfile.output
         output.info("Rewriting files of editable package "
                     "'{}' at '{}'".format(conanfile.name, conanfile.generators_folder))
-        write_generators(conanfile, self._hook_manager)
+        write_generators(conanfile, self._app)
 
         if node.binary == BINARY_EDITABLE_BUILD:
             run_build_method(conanfile, self._hook_manager)
 
         for node in install_node.nodes:
             # Get source of information
             conanfile = node.conanfile
@@ -410,20 +410,20 @@
                 conanfile.cpp.package.set_relative_base_folder(package_folder)
 
                 if is_editable:
                     # Adjust the folders of the layout to consolidate the rootfolder of the
                     # cppinfos inside
 
                     # convert directory entries to be relative to the declared folders.build
-                    build_cppinfo = conanfile.cpp.build.copy()
+                    build_cppinfo = conanfile.cpp.build
                     build_cppinfo.set_relative_base_folder(conanfile.build_folder)
                     conanfile.layouts.build.set_relative_base_folder(conanfile.build_folder)
 
                     # convert directory entries to be relative to the declared folders.source
-                    source_cppinfo = conanfile.cpp.source.copy()
+                    source_cppinfo = conanfile.cpp.source
                     source_cppinfo.set_relative_base_folder(conanfile.source_folder)
                     conanfile.layouts.source.set_relative_base_folder(conanfile.source_folder)
 
                     full_editable_cppinfo = CppInfo()
                     full_editable_cppinfo.merge(source_cppinfo)
                     full_editable_cppinfo.merge(build_cppinfo)
                     # In editables if we defined anything in the cpp infos we want to discard
```

### Comparing `conan-2.0.4/conans/client/loader.py` & `conan-2.0.5/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/loader_txt.py` & `conan-2.0.5/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/migrations.py` & `conan-2.0.5/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/pkg_sign.py` & `conan-2.0.5/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/profile_loader.py` & `conan-2.0.5/conans/client/profile_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,19 @@
         try:
             text = load_user_encoded(profile_path)
         except Exception as e:
             raise ConanException(f"Cannot load profile:\n{e}")
 
         # All profiles will be now rendered with jinja2 as first pass
         base_path = os.path.dirname(profile_path)
+        file_path = os.path.basename(profile_path)
         context = {"platform": platform,
                    "os": os,
                    "profile_dir": base_path,
+                   "profile_name": file_path,
                    "conan_version": conan_version}
         rtemplate = Environment(loader=FileSystemLoader(base_path)).from_string(text)
         text = rtemplate.render(context)
 
         try:
             return self._recurse_load_profile(text, profile_path)
         except ConanException as exc:
```

### Comparing `conan-2.0.4/conans/client/remote_manager.py` & `conan-2.0.5/conans/client/remote_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/__init__.py` & `conan-2.0.5/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/auth_manager.py` & `conan-2.0.5/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/client_routes.py` & `conan-2.0.5/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/conan_requester.py` & `conan-2.0.5/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/file_uploader.py` & `conan-2.0.5/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/rest_client.py` & `conan-2.0.5/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/rest_client_common.py` & `conan-2.0.5/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/rest/rest_client_v2.py` & `conan-2.0.5/conans/client/rest/rest_client_v2.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/source.py` & `conan-2.0.5/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/store/localdb.py` & `conan-2.0.5/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/subsystems.py` & `conan-2.0.5/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/client/userio.py` & `conan-2.0.5/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/conan_server.py` & `conan-2.0.5/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/errors.py` & `conan-2.0.5/conans/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 @contextmanager
 def conanfile_exception_formatter(conanfile_name, func_name):
     """
     Decorator to throw an exception formatted with the line of the conanfile where the error ocurrs.
     """
 
     def _raise_conanfile_exc(e):
-        from conan.api.output import LEVEL_DEBUG, conan_output_level
-        if conan_output_level <= LEVEL_DEBUG:
+        from conan.api.output import LEVEL_DEBUG, ConanOutput
+        if ConanOutput.level_allowed(LEVEL_DEBUG):
             import traceback
             raise ConanExceptionInUserConanfileMethod(traceback.format_exc())
         m = _format_conanfile_exception(conanfile_name, func_name, e)
         raise ConanExceptionInUserConanfileMethod(m)
 
     try:
         yield
```

### Comparing `conan-2.0.4/conans/migrations.py` & `conan-2.0.5/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/build_info.py` & `conan-2.0.5/conans/model/build_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,21 @@
 import copy
 import os
-from collections import OrderedDict
+from collections import OrderedDict, defaultdict
 
 from conan.api.output import ConanOutput
 from conans.errors import ConanException
 
 _DIRS_VAR_NAMES = ["_includedirs", "_srcdirs", "_libdirs", "_resdirs", "_bindirs", "_builddirs",
                    "_frameworkdirs", "_objects"]
 _FIELD_VAR_NAMES = ["_system_libs", "_frameworks", "_libs", "_defines", "_cflags", "_cxxflags",
                     "_sharedlinkflags", "_exelinkflags"]
 _ALL_NAMES = _DIRS_VAR_NAMES + _FIELD_VAR_NAMES
 
 
-class DefaultOrderedDict(OrderedDict):
-
-    def __init__(self, factory):
-        self.factory = factory
-        super(DefaultOrderedDict, self).__init__()
-
-    def __getitem__(self, key):
-        if key not in self.keys():
-            super(DefaultOrderedDict, self).__setitem__(key, self.factory())
-            super(DefaultOrderedDict, self).__getitem__(key).name = key
-        return super(DefaultOrderedDict, self).__getitem__(key)
-
-    def __copy__(self):
-        the_copy = DefaultOrderedDict(self.factory)
-        for key, value in super(DefaultOrderedDict, self).items():
-            the_copy[key] = value
-        return the_copy
-
-
 class MockInfoProperty:
     """
     # TODO: Remove in 2.X
     to mock user_info and env_info
     """
     counter = {}
     package = None
@@ -43,17 +24,17 @@
         self._name = name
 
     @staticmethod
     def message():
         if not MockInfoProperty.counter:
             return
         ConanOutput().warning("Usage of deprecated Conan 1.X features that will be removed in "
-                              "Conan 2.X:")
+                              "Conan 2.X:", warn_tag="deprecated")
         for k, v in MockInfoProperty.counter.items():
-            ConanOutput().warning(f"    '{k}' used in: {', '.join(v)}")
+            ConanOutput().warning(f"    '{k}' used in: {', '.join(v)}", warn_tag="deprecated")
         MockInfoProperty.counter = {}
 
     def __getitem__(self, key):
         MockInfoProperty.counter.setdefault(self._name, set()).add(self.package)
         return []
 
     def __setitem__(self, key, value):
@@ -65,15 +46,15 @@
 
     def __setattr__(self, attr, value):
         if attr != "_name":
             MockInfoProperty.counter.setdefault(self._name, set()).add(self.package)
         return super(MockInfoProperty, self).__setattr__(attr, value)
 
 
-class _Component(object):
+class _Component:
 
     def __init__(self, set_defaults=False):
         # ###### PROPERTIES
         self._generator_properties = None
 
         # ###### DIRECTORIES
         self._includedirs = None  # Ordered list of include paths
@@ -349,132 +330,129 @@
             return None
         try:
             return self._generator_properties[property_name]
         except KeyError:
             pass
 
     def get_init(self, attribute, default):
+        # Similar to dict.setdefault
         item = getattr(self, attribute)
         if item is not None:
             return item
         setattr(self, attribute, default)
         return default
 
+    def merge(self, other, overwrite=False):
+        """
+        @param overwrite:
+        @type other: _Component
+        """
+        def merge_list(o, d):
+            d.extend(e for e in o if e not in d)
+
+        for varname in _ALL_NAMES:
+            other_values = getattr(other, varname)
+            if other_values is not None:
+                if not overwrite:
+                    current_values = self.get_init(varname, [])
+                    merge_list(other_values, current_values)
+                else:
+                    setattr(self, varname, other_values)
+
+        if other.requires:
+            current_values = self.get_init("requires", [])
+            merge_list(other.requires, current_values)
+
+        if other._generator_properties:
+            current_values = self.get_init("_generator_properties", {})
+            current_values.update(other._generator_properties)
+
+    def set_relative_base_folder(self, folder):
+        for varname in _DIRS_VAR_NAMES:
+            origin = getattr(self, varname)
+            if origin is not None:
+                origin[:] = [os.path.join(folder, el) for el in origin]
+        properties = self._generator_properties
+        if properties is not None:
+            modules = properties.get("cmake_build_modules")  # Only this prop at this moment
+            if modules is not None:
+                assert isinstance(modules, list), "cmake_build_modules must be a list"
+                properties["cmake_build_modules"] = [os.path.join(folder, v) for v in modules]
+
+    def deploy_base_folder(self, package_folder, deploy_folder):
+        def relocate(el):
+            rel_path = os.path.relpath(el, package_folder)
+            return os.path.join(deploy_folder, rel_path)
+
+        for varname in _DIRS_VAR_NAMES:
+            origin = getattr(self, varname)
+            if origin is not None:
+                origin[:] = [relocate(f) for f in origin]
+        properties = self._generator_properties
+        if properties is not None:
+            modules = properties.get("cmake_build_modules")  # Only this prop at this moment
+            if modules is not None:
+                assert isinstance(modules, list), "cmake_build_modules must be a list"
+                properties["cmake_build_modules"] = [relocate(f) for f in modules]
 
-class CppInfo(object):
+
+class CppInfo:
 
     def __init__(self, set_defaults=False):
-        self.components = DefaultOrderedDict(lambda: _Component(set_defaults))
+        self.components = defaultdict(lambda: _Component(set_defaults))
         # Main package is a component with None key
-        self.components[None] = _Component(set_defaults)
+        self._package = _Component(set_defaults)
         self._aggregated = None  # A _NewComponent object with all the components aggregated
 
     def __getattr__(self, attr):
-        return getattr(self.components[None], attr)
+        # all cpp_info.xxx of not defined things will go to the global package
+        return getattr(self._package, attr)
 
     def __setattr__(self, attr, value):
-        if attr == "components":
+        if attr in ("components", "_package", "_aggregated"):
             super(CppInfo, self).__setattr__(attr, value)
         else:
-            setattr(self.components[None], attr, value)
+            setattr(self._package, attr, value)
 
     def serialize(self):
-        ret = {}
+        ret = {"root": self._package.serialize()}
         for component_name, info in self.components.items():
-            _name = "root" if component_name is None else component_name
-            ret[_name] = info.serialize()
+            ret[component_name] = info.serialize()
         return ret
 
     @property
     def has_components(self):
-        return len(self.components) > 1
-
-    @property
-    def component_names(self):
-        return filter(None, self.components.keys())
+        return len(self.components) > 0
 
     def merge(self, other, overwrite=False):
         """Merge 'other' into self. 'other' can be an old cpp_info object
         Used to merge Layout source + build cpp objects info (editables)
-        :type other: CppInfo
+        @type other: CppInfo
+        @param other: The other CppInfo to merge
+        @param overwrite: New values from other overwrite the existing ones
         """
-
-        def merge_list(o, d):
-            d.extend(e for e in o if e not in d)
-
-        for varname in _ALL_NAMES:
-            other_values = getattr(other, varname)
-            if other_values is not None:
-                if not overwrite:
-                    current_values = self.components[None].get_init(varname, [])
-                    merge_list(other_values, current_values)
-                else:
-                    setattr(self, varname, other_values)
-        if not self.sysroot and other.sysroot:
-            self.sysroot = other.sysroot
-
-        if other.requires:
-            current_values = self.components[None].get_init("requires", [])
-            merge_list(other.requires, current_values)
-
-        if other._generator_properties:
-            current_values = self.components[None].get_init("_generator_properties", {})
-            current_values.update(other._generator_properties)
-
+        # Global merge
+        self._package.merge(other._package, overwrite)
+        # sysroot only of package, not components, first defined wins
+        self._package.sysroot = self._package.sysroot or other._package.sysroot
         # COMPONENTS
         for cname, c in other.components.items():
-            if cname is None:
-                continue
-            for varname in _ALL_NAMES:
-                other_values = getattr(c, varname)
-                if other_values is not None:
-                    if not overwrite:
-                        current_values = self.components[cname].get_init(varname, [])
-                        merge_list(other_values, current_values)
-                    else:
-                        setattr(self.components[cname], varname, other_values)
-            if c.requires:
-                current_values = self.components[cname].get_init("requires", [])
-                merge_list(c.requires, current_values)
-
-            if c._generator_properties:
-                current_values = self.components[cname].get_init("_generator_properties", {})
-                current_values.update(c._generator_properties)
+            self.components[cname].merge(c, overwrite)
 
     def set_relative_base_folder(self, folder):
-        """Prepend the folder to all the directories"""
+        """Prepend the folder to all the directories definitions, that are relative"""
+        self._package.set_relative_base_folder(folder)
         for component in self.components.values():
-            for varname in _DIRS_VAR_NAMES:
-                origin = getattr(component, varname)
-                if origin is not None:
-                    origin[:] = [os.path.join(folder, el) for el in origin]
-            properties = component._generator_properties
-            if properties is not None:
-                modules = properties.get("cmake_build_modules")  # Only this prop at this moment
-                if modules is not None:
-                    assert isinstance(modules, list), "cmake_build_modules must be a list"
-                    properties["cmake_build_modules"] = [os.path.join(folder, v) for v in modules]
+            component.set_relative_base_folder(folder)
 
     def deploy_base_folder(self, package_folder, deploy_folder):
         """Prepend the folder to all the directories"""
-        def relocate(el):
-            rel_path = os.path.relpath(el, package_folder)
-            return os.path.join(deploy_folder, rel_path)
-
+        self._package.deploy_base_folder(package_folder, deploy_folder)
         for component in self.components.values():
-            for varname in _DIRS_VAR_NAMES:
-                origin = getattr(component, varname)
-                if origin is not None:
-                    origin[:] = [relocate(f) for f in origin]
-            properties = component._generator_properties
-            if properties is not None:
-                modules = properties.get("cmake_build_modules")  # Only this prop at this moment
-                if modules is not None:
-                    assert isinstance(modules, list), "cmake_build_modules must be a list"
-                    properties["cmake_build_modules"] = [relocate(f) for f in modules]
+            component.deploy_base_folder(package_folder, deploy_folder)
 
     def _raise_circle_components_requires_error(self):
         """
         Raise an exception because of a requirements loop detection in components.
         The exception message gives some information about the involved components.
         """
         deps_set = set()
@@ -491,121 +469,90 @@
         """
         Order the components taking into account if they depend on another component in the
         same package (not scoped with ::). First less dependant.
 
         :return: ``OrderedDict`` {component_name: component}
         """
         processed = []  # Names of the components ordered
-        # FIXME: Cache the sort
-        while (len(self.components) - 1) > len(processed):
+        # TODO: Cache the sort
+        while len(self.components) > len(processed):
             cached_processed = processed[:]
             for name, c in self.components.items():
-                if name is None:
-                    continue
                 req_processed = [n for n in c.required_component_names if n not in processed]
                 if not req_processed and name not in processed:
                     processed.append(name)
             # If cached_processed did not change then detected cycle components requirements!
             if cached_processed == processed:
                 self._raise_circle_components_requires_error()
 
         return OrderedDict([(cname, self.components[cname]) for cname in processed])
 
     def aggregated_components(self):
         """Aggregates all the components as global values, returning a new CppInfo"""
         if self._aggregated is None:
             if self.has_components:
                 result = _Component()
-                for n in _ALL_NAMES:  # Initialize all values, from None => []
-                    setattr(result, n, [])  # TODO: This is a bit dirty
                 # Reversed to make more dependant first
-                for name, component in reversed(self.get_sorted_components().items()):
-                    for n in _ALL_NAMES:
-                        if getattr(component, n):
-                            dest = result.get_init(n, [])
-                            dest.extend([i for i in getattr(component, n) if i not in dest])
-
-                    # NOTE: The properties are not aggregated because they might refer only to the
-                    # component like "cmake_target_name" describing the target name FOR THE component
-                    # not the namespace.
-                    if component.requires:
-                        current_values = result.get_init("requires", [])
-                        current_values.extend(component.requires)
-
+                for component in reversed(self.get_sorted_components().values()):
+                    result.merge(component)
+                # NOTE: The properties are not aggregated because they might refer only to the
+                # component like "cmake_target_name" describing the target name FOR THE component
+                # not the namespace.
                 # FIXME: What to do about sysroot?
-                result._generator_properties = copy.copy(self._generator_properties)
+                result._generator_properties = copy.copy(self._package._generator_properties)
             else:
-                result = copy.copy(self.components[None])
+                result = copy.copy(self._package)
             self._aggregated = CppInfo()
-            self._aggregated.components[None] = result
+            self._aggregated._package = result
         return self._aggregated
 
     def check_component_requires(self, conanfile):
         """ quality check for component requires:
         - Check that all recipe ``requires`` are used if consumer recipe explicit opt-in to use
           component requires
         - Check that component external dep::comp dependency "dep" is a recipe "requires"
         - Check that every internal component require actually exist
         It doesn't check that external components do exist
         """
-        if not self.has_components and not self.requires:
+        if not self.has_components and not self._package.requires:
             return
         # Accumulate all external requires
-        external = set()
-        internal = set()
+        external = set(r.split("::")[0] for r in self._package.requires if "::" in r)
+        internal = set(r for r in self._package.requires if "::" not in r)
         # TODO: Cache this, this is computed in different places
         for key, comp in self.components.items():
             external.update(r.split("::")[0] for r in comp.requires if "::" in r)
             internal.update(r for r in comp.requires if "::" not in r)
 
         missing_internal = list(internal.difference(self.components))
         if missing_internal:
             raise ConanException(f"{conanfile}: Internal components not found: {missing_internal}")
         if not external:
             return
-        # Only direct host dependencies can be used with components
-        direct_dependencies = [d.ref.name
-                               for d, _ in conanfile.dependencies.filter({"direct": True,
-                                                                          "build": False,
-                                                                          "test": False}).items()]
+        # Only direct host (not test) dependencies can define required components
+        direct_dependencies = [d.ref.name for d in conanfile.requires.values()
+                               if not d.build and not d.is_test and d.visible]
+
         for e in external:
             if e not in direct_dependencies:
                 raise ConanException(
                     f"{conanfile}: required component package '{e}::' not in dependencies")
         # TODO: discuss if there are cases that something is required but not transitive
         for e in direct_dependencies:
             if e not in external:
                 raise ConanException(
                     f"{conanfile}: Required package '{e}' not in component 'requires'")
 
-    def copy(self):
-        # Only used at the moment by layout() editable merging build+source .cpp data
-        ret = CppInfo()
-        ret._generator_properties = copy.copy(self._generator_properties)
-        ret.components = DefaultOrderedDict(lambda: _Component())
-        for comp_name in self.components:
-            ret.components[comp_name] = copy.copy(self.components[comp_name])
-        return ret
-
     @property
     def required_components(self):
         """Returns a list of tuples with (require, component_name) required by the package
         If the require is internal (to another component), the require will be None"""
         # FIXME: Cache the value
         # First aggregate without repetition, respecting the order
-        ret = []
+        ret = [r for r in self._package.requires]
         for comp in self.components.values():
             for r in comp.requires:
                 if r not in ret:
                     ret.append(r)
         # Then split the names
         ret = [r.split("::") if "::" in r else (None, r) for r in ret]
         return ret
-
-    def __str__(self):
-        ret = []
-        for cname, c in self.components.items():
-            for n in _ALL_NAMES:
-                ret.append("Component: '{}' "
-                           "Var: '{}' "
-                           "Value: '{}'".format(cname, n, getattr(c, n)))
-        return "\n".join(ret)
```

### Comparing `conan-2.0.4/conans/model/conan_file.py` & `conan-2.0.5/conans/model/conan_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from conans.model.build_info import MockInfoProperty
 from conans.model.conf import Conf
 from conans.model.dependencies import ConanFileDependencies
 from conans.model.layout import Folders, Infos, Layouts
 from conans.model.options import Options
 
 from conans.model.requires import Requirements
+from conans.model.settings import Settings
 
 
 class ConanFile:
     """
     The base class for all package recipes
     """
 
@@ -117,25 +118,40 @@
         self.folders = Folders()
         self.cpp = Infos()
         self.layouts = Layouts()
 
     def serialize(self):
         result = {}
 
-        for a in ("url", "license", "author", "description", "topics", "homepage", "build_policy",
-                  "upload_policy",
-                  "revision_mode", "provides", "deprecated", "win_bash", "win_bash_run"):
-            v = getattr(self, a)
+        for a in ("name", "user", "channel", "url", "license",
+                  "author", "description", "homepage", "build_policy", "upload_policy",
+                  "revision_mode", "provides", "deprecated", "win_bash", "win_bash_run",
+                  "default_options", "options_description",):
+            v = getattr(self, a, None)
             if v is not None:
                 result[a] = v
-
+        if self.version is not None:
+            result["version"] = str(self.version)
+        if self.topics is not None:
+            result["topics"] = list(self.topics)
         result["package_type"] = str(self.package_type)
-        result["settings"] = self.settings.serialize()
+
+        settings = self.settings
+        if settings is not None:
+            result["settings"] = settings.serialize() if isinstance(settings, Settings) else list(settings)
+
         result["options"] = self.options.serialize()
+        result["options_definitions"] = self.options.possible_values
+
+        if self.generators is not None:
+            result["generators"] = list(self.generators)
+        if self.license is not None:
+            result["license"] = list(self.license) if not isinstance(self.license, str) else self.license
 
+        result["requires"] = self.requires.serialize()
         if hasattr(self, "python_requires"):
             result["python_requires"] = [r.repr_notime() for r in self.python_requires.all_refs()]
         result["system_requires"] = self.system_requires
 
         result["recipe_folder"] = self.recipe_folder
         result["source_folder"] = self.source_folder
         result["build_folder"] = self.build_folder
```

### Comparing `conan-2.0.4/conans/model/conanfile_interface.py` & `conan-2.0.5/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/conf.py` & `conan-2.0.5/conans/model/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from conans.errors import ConanException
 from conans.model.recipe_ref import ref_matches
 
 BUILT_IN_CONFS = {
     "core:required_conan_version": "Raise if current version does not match the defined range.",
     "core:non_interactive": "Disable interactive user input, raises error if input necessary",
+    "core:skip_warnings": "Do not show warnings in this list",
     "core:default_profile": "Defines the default host profile ('default' by default)",
     "core:default_build_profile": "Defines the default build profile (None by default)",
     "core:allow_uppercase_pkg_names": "Temporarily (will be removed in 2.X) allow uppercase names",
     "core.version_ranges:resolve_prereleases": "Whether version ranges can resolve to pre-releases or not",
     "core.upload:retry": "Number of retries in case of failure when uploading to Conan server",
     "core.upload:retry_wait": "Seconds to wait between upload attempts to Conan server",
     "core.download:parallel": "Number of concurrent threads to download packages",
@@ -262,18 +263,15 @@
         """
         :type other: Conf
         """
         return other._values == self._values
 
     def validate(self):
         for conf in self._values:
-            if conf.startswith("tools") or conf.startswith("core"):
-                if conf not in BUILT_IN_CONFS:
-                    raise ConanException(f"Unknown conf '{conf}'. Use 'conan config list' to "
-                                         "display existing configurations")
+            self._check_conf_name(conf)
 
     def items(self):
         # FIXME: Keeping backward compatibility
         for k, v in self._values.items():
             yield k, v.value
 
     def get(self, conf_name, default=None, check_type=None):
@@ -282,17 +280,15 @@
 
         :param conf_name: Name of the configuration.
         :param default: Default value in case of conf does not have the conf_name key.
         :param check_type: Check the conf type(value) is the same as the given by this param.
                            There are two default smart conversions for bool and str types.
         """
         # Skipping this check only the user.* configurations
-        if USER_CONF_PATTERN.match(conf_name) is None and conf_name not in BUILT_IN_CONFS:
-            raise ConanException(f"[conf] '{conf_name}' does not exist in configuration list. "
-                                 f" Run 'conan config list' to see all the available confs.")
+        self._check_conf_name(conf_name)
 
         conf_value = self._values.get(conf_name)
         if conf_value:
             v = conf_value.value
             # Some smart conversions
             if check_type is bool and not isinstance(v, bool):
                 # Perhaps, user has introduced a "false", "0" or even "off"
@@ -475,14 +471,20 @@
                 result.define(conf_name, value)
         return result
 
     def set_relative_base_folder(self, folder):
         for v in self._values.values():
             v.set_relative_base_folder(folder)
 
+    @staticmethod
+    def _check_conf_name(conf):
+        if USER_CONF_PATTERN.match(conf) is None and conf not in BUILT_IN_CONFS:
+            raise ConanException(f"[conf] '{conf}' does not exist in configuration list. "
+                                 f" Run 'conan config list' to see all the available confs.")
+
 
 class ConfDefinition:
 
     # Order is important, "define" must be latest
     actions = (("+=", "append"), ("=+", "prepend"),
                ("=!", "unset"), ("*=", "update"), ("=", "define"))
```

### Comparing `conan-2.0.4/conans/model/dependencies.py` & `conan-2.0.5/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/graph_lock.py` & `conan-2.0.5/conans/model/graph_lock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 from collections import OrderedDict
 
-from conans.client.graph.graph import RECIPE_VIRTUAL, RECIPE_CONSUMER, CONTEXT_BUILD
+from conan.api.output import ConanOutput
+from conans.client.graph.graph import RECIPE_VIRTUAL, RECIPE_CONSUMER, CONTEXT_BUILD, Overrides
 from conans.errors import ConanException
 from conans.model.recipe_ref import RecipeReference
 from conans.util.files import load, save
 
 LOCKFILE = "conan.lock"
 LOCKFILE_VERSION = "0.5"
 
@@ -83,14 +84,15 @@
 class Lockfile(object):
 
     def __init__(self, deps_graph=None, lock_packages=False):
         self._requires = _LockRequires()
         self._python_requires = _LockRequires()
         self._build_requires = _LockRequires()
         self._alias = {}
+        self._overrides = Overrides()
         self.partial = False
 
         if deps_graph is None:
             return
 
         self.update_lock(deps_graph, lock_packages)
 
@@ -108,14 +110,15 @@
             pids = {graph_node.package_id: graph_node.prev} if lock_packages else None
             if graph_node.context == CONTEXT_BUILD:
                 self._build_requires.add(graph_node.ref, pids)
             else:
                 self._requires.add(graph_node.ref, pids)
 
         self._alias.update(deps_graph.aliased)
+        self._overrides.update(deps_graph.overrides())
 
         self._requires.sort()
         self._build_requires.sort()
         self._python_requires.sort()
 
     @staticmethod
     def load(path):
@@ -142,14 +145,16 @@
     def merge(self, other):
         """
         :type other: Lockfile
         """
         self._requires.merge(other._requires)
         self._build_requires.merge(other._build_requires)
         self._python_requires.merge(other._python_requires)
+        self._alias.update(other._alias)
+        self._overrides.update(other._overrides)
 
     def add(self, requires=None, build_requires=None, python_requires=None):
         """ adding new things manually will trigger the sort() of the locked list, so lockfiles
         alwasys keep the ordered lists. This means that for some especial edge cases it might
         be necessary to allow removing from a lockfile, for example to test an older version
         than the one locked (in general adding works better for moving forward to newer versions)
         """
@@ -180,14 +185,16 @@
         if "build_requires" in data:
             graph_lock._build_requires = _LockRequires.deserialize(data["build_requires"])
         if "python_requires" in data:
             graph_lock._python_requires = _LockRequires.deserialize(data["python_requires"])
         if "alias" in data:
             graph_lock._alias = {RecipeReference.loads(k): RecipeReference.loads(v)
                                  for k, v in data["alias"].items()}
+        if "overrides" in data:
+            graph_lock._overrides = Overrides.deserialize(data["overrides"])
         return graph_lock
 
     def serialize(self):
         """ returns the object serialized as a dict of plain python types
         that can be converted to json
         """
         result = {"version": LOCKFILE_VERSION}
@@ -195,22 +202,42 @@
             result["requires"] = self._requires.serialize()
         if self._build_requires:
             result["build_requires"] = self._build_requires.serialize()
         if self._python_requires:
             result["python_requires"] = self._python_requires.serialize()
         if self._alias:
             result["alias"] = {repr(k): repr(v) for k, v in self._alias.items()}
+        if self._overrides:
+            result["overrides"] = self._overrides.serialize()
         return result
 
     def resolve_locked(self, node, require, resolve_prereleases):
         if require.build or node.context == CONTEXT_BUILD:
             locked_refs = self._build_requires.refs()
         else:
             locked_refs = self._requires.refs()
-        self._resolve(require, locked_refs, resolve_prereleases)
+        self._resolve_overrides(require)
+        try:
+            self._resolve(require, locked_refs, resolve_prereleases)
+        except ConanException:
+            overrides = self._overrides.get(require.ref)
+            if overrides is not None and len(overrides) > 1:
+                msg = f"Override defined for {require.ref}, but multiple possible overrides" \
+                      f" {overrides}. You might need to apply the 'conan graph build-order'" \
+                      f" overrides for correctly building this package with this lockfile"
+                ConanOutput().error(msg)
+            raise
+
+    def _resolve_overrides(self, require):
+        existing = self._overrides.get(require.ref)
+        if existing is not None and len(existing) == 1:
+            require.overriden_ref = require.ref  # Store that the require has been overriden
+            ref = next(iter(existing))
+            require.ref = ref
+            require.override_ref = ref
 
     def resolve_prev(self, node):
         if node.context == CONTEXT_BUILD:
             prevs = self._build_requires.get(node.ref)
         else:
             prevs = self._requires.get(node.ref)
         if prevs:
@@ -226,30 +253,31 @@
                 if version_range.contains(m.version, resolve_prereleases):
                     require.ref = m
                     break
             else:
                 if not self.partial:
                     raise ConanException(f"Requirement '{ref}' not in lockfile")
         else:
-            alias = require.alias
-            if alias:
-                locked_alias = self._alias.get(alias)
-                if locked_alias is not None:
-                    require.ref = locked_alias
-                elif not self.partial:
-                    raise ConanException(f"Requirement alias '{alias}' not in lockfile")
             ref = require.ref
             if ref.revision is None:
                 for m in matches:
                     if m.version == ref.version:
                         require.ref = m
                         break
                 else:
                     if not self.partial:
                         raise ConanException(f"Requirement '{ref}' not in lockfile")
             else:
                 if ref not in matches and not self.partial:
                     raise ConanException(f"Requirement '{repr(ref)}' not in lockfile")
 
+    def replace_alias(self, require, alias):
+        locked_alias = self._alias.get(alias)
+        if locked_alias is not None:
+            require.ref = locked_alias
+            return True
+        elif not self.partial:
+            raise ConanException(f"Requirement alias '{alias}' not in lockfile")
+
     def resolve_locked_pyrequires(self, require, resolve_prereleases=None):
         locked_refs = self._python_requires.refs()  # CHANGE
         self._resolve(require, locked_refs, resolve_prereleases)
```

### Comparing `conan-2.0.4/conans/model/info.py` & `conan-2.0.5/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/layout.py` & `conan-2.0.5/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/manifest.py` & `conan-2.0.5/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/options.py` & `conan-2.0.5/conans/model/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,16 +387,18 @@
             self_options._deps_package_options.setdefault(pattern,
                                                           _PackageOptions()).update_options(options)
 
         # compute now the necessary to propagate all down - self + self deps
         upstream_options = Options()
         for pattern, options in down_options._deps_package_options.items():
             if ref_matches(own_ref, pattern, is_consumer=is_consumer):
-                # Remove the exact match to this package, don't further propagate up
-                continue
+                # Remove the exact match-name to this package, don't further propagate up
+                pattern_name = pattern.split("/", 1)[0]
+                if "*" not in pattern_name:
+                    continue
             self._deps_package_options.setdefault(pattern, _PackageOptions()).update_options(options)
 
         upstream_options._deps_package_options = self._deps_package_options
         # When the upstream is computed, the current dependencies are invalidated, so users will
         # not be able to do ``self.options["mydep"]`` because it will be empty. self.dependencies
         # is the way to access dependencies (in other methods)
         self._deps_package_options = {}
```

### Comparing `conan-2.0.4/conans/model/package_ref.py` & `conan-2.0.5/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/pkg_type.py` & `conan-2.0.5/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/profile.py` & `conan-2.0.5/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/recipe_ref.py` & `conan-2.0.5/conans/model/recipe_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,17 @@
                 raise ConanException(f"Conan packages names '{self_str}' must be all lowercase")
             else:
                 ConanOutput().warning(f"Package name '{self_str}' has uppercase, and has been "
                                       "allowed by temporary config. This will break in later 2.X")
         if len(self_str) > 200:
             raise ConanException(f"Package reference too long >200 {self_str}")
         if not allow_uppercase:
-            validation_pattern = re.compile(r"^[a-z0-9_][a-z0-9_+.-]{1,100}$")
+            validation_pattern = re.compile(r"^[a-z0-9_][a-z0-9_+.-]{1,100}\Z")
         else:
-            validation_pattern = re.compile(r"^[a-zA-Z0-9_][a-zA-Z0-9_+.-]{1,100}$")
+            validation_pattern = re.compile(r"^[a-zA-Z0-9_][a-zA-Z0-9_+.-]{1,100}\Z")
         if validation_pattern.match(self.name) is None:
             raise ConanException(f"Invalid package name '{self.name}'")
         if validation_pattern.match(str(self.version)) is None:
             raise ConanException(f"Invalid package version '{self.version}'")
         if self.user and validation_pattern.match(self.user) is None:
             raise ConanException(f"Invalid package user '{self.user}'")
         if self.channel and validation_pattern.match(self.channel) is None:
```

### Comparing `conan-2.0.4/conans/model/requires.py` & `conan-2.0.5/conans/model/requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         self._transitive_libs = transitive_libs
         self._test = test
         self._package_id_mode = package_id_mode
         self._force = force
         self._override = override
         self._direct = direct
         self.options = options
+        # Meta and auxiliary information
+        self.overriden_ref = None  # to store if the requirement has been overriden (store old ref)
+        self.override_ref = None  # to store if the requirement has been overriden (store new ref)
+        self.is_test = test  # to store that it was a test, even if used as regular requires too
 
     @property
     def skip(self):
         return not (self.headers or self.libs or self.run or self.build)
 
     @staticmethod
     def _default_if_none(field, default_value):
@@ -138,14 +142,20 @@
 
     def __str__(self):
         traits = 'build={}, headers={}, libs={}, '  \
                  'run={}, visible={}'.format(self.build, self.headers, self.libs, self.run,
                                              self.visible)
         return "{}, Traits: {}".format(self.ref, traits)
 
+    def serialize(self):
+        serializable = ("ref", "run", "libs", "skip", "test", "force", "direct", "build",
+                        "transitive_headers", "transitive_libs", "headers",
+                        "package_id_mode", "visible")
+        return {attribute: str(getattr(self, attribute)) for attribute in serializable}
+
     def copy_requirement(self):
         return Requirement(self.ref, headers=self.headers, libs=self.libs, build=self.build,
                            run=self.run, visible=self.visible,
                            transitive_headers=self.transitive_headers,
                            transitive_libs=self.transitive_libs)
 
     @property
@@ -184,15 +194,15 @@
         elif pkg_type is PackageType.STATIC:
             set_if_none("_run", False)
         elif pkg_type is PackageType.HEADER:
             set_if_none("_run", False)
             set_if_none("_libs", False)
             set_if_none("_headers", True)
         elif pkg_type is PackageType.BUILD_SCRIPTS:
-            set_if_none("_run", False)
+            set_if_none("_run", True)
             set_if_none("_libs", False)
             set_if_none("_headers", False)
             set_if_none("_visible", False)  # Conflicts might be allowed for this kind of package
 
         src_pkg_type = src_node.conanfile.package_type
         if src_pkg_type is PackageType.HEADER:
             set_if_none("_transitive_headers", True)
@@ -207,15 +217,15 @@
         we consider the requires equal, so they can conflict"""
         return (self.ref.name == other.ref.name and self.build == other.build and
                 (self.override or  # an override with same name and context, always match
                  (self.headers and other.headers) or
                  (self.libs and other.libs) or
                  (self.run and other.run) or
                  (self.visible and other.visible) or
-                 (self.ref == other.ref)))
+                 (self.ref == other.ref and self.options == other.options)))
 
     def aggregate(self, other):
         """ when closing loop and finding the same dependency on a node, the information needs
         to be aggregated
         :param other: is the existing Require that the current node has, which information has to be
         appended to "self", which is the requires that is being propagated to the current node
         from upstream
@@ -381,18 +391,19 @@
 
 
 class BuildRequirements:
     # Just a wrapper around requires for backwards compatibility with self.build_requires() syntax
     def __init__(self, requires):
         self._requires = requires
 
-    def __call__(self, ref, package_id_mode=None, visible=False, run=None, options=None):
+    def __call__(self, ref, package_id_mode=None, visible=False, run=None, options=None,
+                 override=None):
         # TODO: Check which arguments could be user-defined
         self._requires.build_require(ref, package_id_mode=package_id_mode, visible=visible, run=run,
-                                     options=options)
+                                     options=options, override=override)
 
 
 class ToolRequirements:
     # Just a wrapper around requires for backwards compatibility with self.build_requires() syntax
     def __init__(self, requires):
         self._requires = requires
 
@@ -474,15 +485,15 @@
         ref = RecipeReference.loads(str_ref)
         req = Requirement(ref, **kwargs)
         if self._requires.get(req):
             raise ConanException("Duplicated requirement: {}".format(ref))
         self._requires[req] = req
 
     def build_require(self, ref, raise_if_duplicated=True, package_id_mode=None, visible=False,
-                      run=None, options=None):
+                      run=None, options=None, override=None):
         """
              Represent a generic build require, could be a tool, like "cmake" or a bundle of build
              scripts.
 
              visible = False => Only the direct consumer can see it, won't conflict
              build = True => They run in the build machine (e.g cmake)
              libs = False => We won't link with it, is a tool, no propagate the libs.
@@ -490,15 +501,15 @@
              run = None => It will be determined by the package_type of the ref
         """
         if ref is None:
             return
         # FIXME: This raise_if_duplicated is ugly, possibly remove
         ref = RecipeReference.loads(ref)
         req = Requirement(ref, headers=False, libs=False, build=True, run=run, visible=visible,
-                          package_id_mode=package_id_mode, options=options)
+                          package_id_mode=package_id_mode, options=options, override=override)
 
         if raise_if_duplicated and self._requires.get(req):
             raise ConanException("Duplicated requirement: {}".format(ref))
         self._requires[req] = req
 
     def override(self, ref):
         req = Requirement(ref)
@@ -549,7 +560,10 @@
                           package_id_mode=package_id_mode, options=options, override=override)
         if raise_if_duplicated and self._requires.get(req):
             raise ConanException("Duplicated requirement: {}".format(ref))
         self._requires[req] = req
 
     def __repr__(self):
         return repr(self._requires.values())
+
+    def serialize(self):
+        return [v.serialize() for v in self._requires.values()]
```

### Comparing `conan-2.0.4/conans/model/rest_routes.py` & `conan-2.0.5/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/settings.py` & `conan-2.0.5/conans/model/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,20 @@
 
     def validate(self):
         if self._value is None and None not in self._definition:
             raise ConanException("'%s' value not defined" % self._name)
         if isinstance(self._definition, dict):
             self._definition[self._value].validate()
 
-    def get_definition(self):
+    def possible_values(self):
         if isinstance(self._definition, list):
-            return [e if e != 'None' else None for e in self.values_range]
+            return self.values_range.copy()
         ret = {}
         for key, value in self._definition.items():
-            ret[key] = value.get_definition()
+            ret[key] = value.possible_values()
         return ret
 
     def rm_safe(self, name):
         """ Iterates all possible subsettings, calling rm_safe() for all of them. If removing
         "compiler.cppstd", this will iterate msvc, gcc, clang, etc, calling rm_safe(cppstd) for
         all of them"""
         if isinstance(self._definition, list):
@@ -171,14 +171,17 @@
 
 
 class Settings(object):
     def __init__(self, definition=None, name="settings", parent_value="settings"):
         if parent_value is None and definition:
             raise ConanException("settings.yml: null setting can't have subsettings")
         definition = definition or {}
+        if not isinstance(definition, dict):
+            val = "" if parent_value == "settings" else f"={parent_value}"
+            raise ConanException(f"Invalid settings.yml format: '{name}{val}' is not a dictionary")
         self._name = name  # settings, settings.compiler
         self._parent_value = parent_value  # gcc, x86
         self._data = {k: SettingsItem(v, "%s.%s" % (name, k))
                       for k, v in definition.items()}
         self._frozen = False
 
     def serialize(self):
@@ -334,15 +337,14 @@
             # It is important to discard None values, so migrations in settings can be done
             # without breaking all existing packages SHAs, by adding a first None option
             # that doesn't change the final sha
             if value is not None:
                 result.append("%s=%s" % (name, value))
         return '\n'.join(result)
 
-    def get_definition(self):
-        """Check the range of values of the definition of a setting. e.g:
-           get_definition_values("compiler.gcc.version") """
-
+    def possible_values(self):
+        """Check the range of values of the definition of a setting
+        """
         ret = {}
         for key, element in self._data.items():
-            ret[key] = element.get_definition()
+            ret[key] = element.possible_values()
         return ret
```

### Comparing `conan-2.0.4/conans/model/version.py` & `conan-2.0.5/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/model/version_range.py` & `conan-2.0.5/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/paths/__init__.py` & `conan-2.0.5/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/pylint_plugin.py` & `conan-2.0.5/conans/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/search/query_parse.py` & `conan-2.0.5/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/search/search.py` & `conan-2.0.5/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/conftest.py` & `conan-2.0.5/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/artifactory.py` & `conan-2.0.5/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/mocks.py` & `conan-2.0.5/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/profiles.py` & `conan-2.0.5/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/scm.py` & `conan-2.0.5/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/server_launcher.py` & `conan-2.0.5/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/test_files.py` & `conan-2.0.5/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/test/utils/tools.py` & `conan-2.0.5/conans/test/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,14 +699,30 @@
         for r, kind in requires.items():
             for req in reqs:
                 if req.startswith(r) and req.endswith(kind):
                     break
             else:
                 raise AssertionError(f"Cant find {r}-{kind} in {reqs}")
 
+    def assert_overrides(self, overrides):
+        """ parses the current command output, and extract the first "Requirements" section
+        """
+        lines = self.out.splitlines()
+        header = "Overrides"
+        line_req = lines.index(header)
+        reqs = []
+        for line in lines[line_req+1:]:
+            if not line.startswith("    "):
+                break
+            reqs.append(line.strip())
+        for r, o in overrides.items():
+            msg = f"{r}: {o}"
+            if msg not in reqs:
+                raise AssertionError(f"Cant find {msg} in {reqs}")
+
     def assert_listed_binary(self, requires, build=False, test=False, test_package=False):
         """ parses the current command output, and extract the second "Requirements" section
         belonging to the computed package binaries
         """
         lines = self.out.splitlines()
         if test_package:
             line_req = lines.index("======== Launching test_package ========")
```

### Comparing `conan-2.0.4/conans/util/config_parser.py` & `conan-2.0.5/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/dates.py` & `conan-2.0.5/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/encrypt.py` & `conan-2.0.5/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/env.py` & `conan-2.0.5/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/files.py` & `conan-2.0.5/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/locks.py` & `conan-2.0.5/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/runners.py` & `conan-2.0.5/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/sha.py` & `conan-2.0.5/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/conans/util/windows.py` & `conan-2.0.5/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.4/setup.py` & `conan-2.0.5/setup.py`

 * *Files identical despite different names*

