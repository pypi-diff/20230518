# Comparing `tmp/trivial_torch_tools-0.6.0.tar.gz` & `tmp/trivial_torch_tools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trivial_torch_tools-0.6.0.tar", last modified: Thu May 18 17:00:08 2023, max compression
+gzip compressed data, was "trivial_torch_tools-0.6.1.tar", last modified: Thu May 18 17:11:52 2023, max compression
```

## Comparing `trivial_torch_tools-0.6.0.tar` & `trivial_torch_tools-0.6.1.tar`

### file list

```diff
@@ -1,417 +1,417 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.603284 trivial_torch_tools-0.6.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-18 17:00:08.603112 trivial_torch_tools-0.6.0/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-18 17:00:08.603328 trivial_torch_tools-0.6.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1453 2023-05-18 16:49:02.000000 trivial_torch_tools-0.6.0/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.491886 trivial_torch_tools-0.6.0/trivial_torch_tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.492954 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-05-18 16:57:30.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.493278 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4319 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.485303 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.495486 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      424 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.496890 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.498091 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.498588 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.504052 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.505298 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/main.py.log
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.505976 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.506219 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.507272 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    10922 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.509349 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.509572 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.509925 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.511860 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.513256 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.515739 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.523524 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.526679 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.485001 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.526904 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.483750 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.483915 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.528521 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.531344 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.533117 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.534781 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.535230 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.484664 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.535430 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.535638 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.535865 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.535983 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.536171 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.536421 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.536508 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.536990 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.537206 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.537317 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.539864 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.540895 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.541042 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.542444 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.544592 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.545397 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.545794 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.546193 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.546309 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.547516 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.548335 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.549371 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.551339 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.554568 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.555640 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.485707 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.485747 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.555851 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.556138 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3435 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.485911 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.556358 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      821 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.556759 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      656 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    11162 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.557119 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8109 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6-py3-none-any.whl
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7986 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6.tar.gz
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.557799 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    11225 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.559791 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8164 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.558667 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.560342 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.561429 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.562078 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.562917 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.564873 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.571723 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.574721 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.489108 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.575503 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.486803 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.487601 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.576424 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.577558 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.579002 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.579699 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.580176 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.488737 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.580357 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.580694 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.580930 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.581052 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.581706 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.582111 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.582222 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.582318 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.582409 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.582500 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.585898 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.587861 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.588650 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.589165 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.589672 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.593790 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.594228 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.594348 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      497 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)       28 2023-05-18 16:28:26.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.594517 trivial_torch_tools-0.6.0/trivial_torch_tools/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-05-18 16:41:27.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.598679 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.602748 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3269 2023-05-18 16:41:55.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/core.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6866 2023-05-18 16:51:21.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/generics.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1874 2023-05-18 16:43:16.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/image.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1571 2023-05-18 16:49:35.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/main.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1494 2023-05-18 16:49:45.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/misc.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8980 2023-05-18 16:42:09.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/model.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2121 2023-05-18 16:42:34.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/one_hots.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4653 2023-05-18 16:41:54.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/core.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8875 2023-05-18 16:58:54.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/generics.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:25:43.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/image.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      906 2023-05-18 16:43:52.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/main.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1920 2023-05-18 16:43:44.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/misc.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8906 2023-05-18 16:42:07.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/model.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1746 2023-05-18 16:42:16.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/contents/one_hots.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      380 2023-05-18 16:48:39.000000 trivial_torch_tools-0.6.0/trivial_torch_tools/settings.json
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:00:08.492781 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-18 17:00:08.000000 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)    31705 2023-05-18 17:00:08.000000 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-18 17:00:08.000000 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 17:00:08.000000 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2023-05-18 17:00:08.000000 trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/top_level.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.729142 trivial_torch_tools-0.6.1/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-18 17:11:52.728575 trivial_torch_tools-0.6.1/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-18 17:11:52.729343 trivial_torch_tools-0.6.1/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1453 2023-05-18 16:49:02.000000 trivial_torch_tools-0.6.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.637812 trivial_torch_tools-0.6.1/trivial_torch_tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.638665 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-05-18 16:57:30.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.639078 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4319 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.633631 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.640465 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      424 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.641333 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.642146 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.642525 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.645566 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.646250 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.646728 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.646906 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.647065 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10922 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.647437 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.647557 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.647853 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.648463 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.649158 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.649618 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.653868 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.656252 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.633308 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.656430 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.631687 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.631853 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.657576 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.658753 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.659902 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.660674 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.660995 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.632932 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.661153 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.661748 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.661982 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.663978 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.664235 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.664558 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.664673 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.664776 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.665696 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.665821 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.668918 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.671386 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.671619 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.672128 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.672643 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.674142 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.674557 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.674950 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.675086 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-18 16:48:03.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.676859 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.677840 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.679631 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.680084 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.684627 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.685605 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.634037 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.634082 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.685935 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.686252 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3435 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.634253 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.686433 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      821 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.688311 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      656 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11162 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.688818 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8109 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6-py3-none-any.whl
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7986 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6.tar.gz
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.689834 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11225 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.691359 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8164 2023-05-18 16:57:34.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.691193 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.691752 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.692139 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.692753 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.693498 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.694060 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.700744 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.703614 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.636469 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.703786 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.635160 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.635318 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.705155 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.708718 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.710383 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.711029 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.711296 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.636204 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.711434 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.711856 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.712078 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.712230 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.713224 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.713567 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.713703 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.713806 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.713911 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.714021 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.717982 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.719378 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.719834 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.720251 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.721201 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.721593 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.721915 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.723113 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      497 2023-05-18 16:30:46.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/tests/test.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      319 2023-05-18 17:09:56.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.723435 trivial_torch_tools-0.6.1/trivial_torch_tools/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      409 2023-05-18 17:11:41.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.726386 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.728363 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3269 2023-05-18 16:41:55.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/core.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6827 2023-05-18 17:11:42.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/generics.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1874 2023-05-18 16:43:16.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/image.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1571 2023-05-18 16:49:35.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2678 2023-05-18 17:11:42.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/misc.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8980 2023-05-18 16:42:09.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2121 2023-05-18 16:42:34.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/one_hots.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4653 2023-05-18 16:41:54.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/core.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8875 2023-05-18 16:58:54.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/generics.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1328 2023-05-18 16:25:43.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/image.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      906 2023-05-18 16:43:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/main.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2821 2023-05-18 17:11:17.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/misc.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8906 2023-05-18 16:42:07.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/model.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1746 2023-05-18 16:42:16.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/contents/one_hots.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      380 2023-05-18 16:48:39.000000 trivial_torch_tools-0.6.1/trivial_torch_tools/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-18 17:11:52.638546 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3039 2023-05-18 17:11:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    31705 2023-05-18 17:11:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-18 17:11:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-05-18 17:11:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/requires.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       20 2023-05-18 17:11:52.000000 trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/top_level.txt
```

### Comparing `trivial_torch_tools-0.6.0/PKG-INFO` & `trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trivial_torch_tools
-Version: 0.6.0
+Name: trivial-torch-tools
+Version: 0.6.1
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `trivial_torch_tools-0.6.0/setup.py` & `trivial_torch_tools-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__init__.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/.gitignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/README.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/commands`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/project/purge`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/shell`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/commands/start`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/license.txt`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/main/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/poetry.lock`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/run/tests.ps1`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/file_system_py/tests/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/.gitignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/README.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/commands`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/project/purge`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/shell`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/commands/start`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/__init__.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/setup.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__init__.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6-py3-none-any.whl` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6.tar.gz` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6.tar.gz`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/license.txt`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/setup.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/__init__.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/PKG-INFO` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/poetry.lock`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml` & `trivial_torch_tools-0.6.1/trivial_torch_tools/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/core.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/core.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/image.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/image.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/main.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/misc.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/misc.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May 18 16:43:44 2023 UTC, .py size: 1920 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,168 @@
-00000000: 550d 0d0a 0000 0000 c055 6664 8007 0000  U........Ufd....
+00000000: 550d 0d0a 0000 0000 355c 6664 050b 0000  U.......5\fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
+00000020: 0003 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 6d04 5a04 0100 6403  Z.d.d.l.m.Z...d.
-00000050: 6404 8400 5a05 6405 6406 8400 5a06 6409  d...Z.d.d...Z.d.
-00000060: 6407 6408 8401 5a07 6402 5300 290a e900  d.d...Z.d.S.)...
-00000070: 0000 0029 01da 0b4f 7264 6572 6564 4469  ...)...OrderedDi
-00000080: 6374 4e63 0300 0000 0000 0000 0000 0000  ctNc............
-00000090: 0700 0000 0500 0000 6300 0000 7346 0000  ........c...sF..
-000000a0: 0064 0164 026c 006d 017d 0301 0074 027c  .d.d.l.m.}...t.|
-000000b0: 037c 007c 0283 027c 037c 017c 0283 0283  .|.|...|.|.|....
-000000c0: 027d 047c 0444 005d 1a5c 027d 057d 0674  .}.|.D.].\.}.}.t
-000000d0: 037c 0583 0174 037c 0683 0166 0256 0001  .|...t.|...f.V..
-000000e0: 0071 2664 0053 0029 034e e901 0000 0029  .q&d.S.).N.....)
-000000f0: 01da 0662 756e 646c 6529 04da 0867 656e  ...bundle)...gen
-00000100: 6572 6963 7372 0400 0000 da03 7a69 70da  ericsr......zip.
-00000110: 0974 6f5f 7465 6e73 6f72 2907 da06 696e  .to_tensor)...in
-00000120: 7075 7473 da07 6f75 7470 7574 73da 0a62  puts..outputs..b
-00000130: 6174 6368 5f73 697a 6572 0400 0000 5a07  atch_sizer....Z.
-00000140: 6261 7463 6865 735a 1065 6163 685f 696e  batchesZ.each_in
-00000150: 7075 745f 6261 7463 685a 1165 6163 685f  put_batchZ.each_
-00000160: 6f75 7470 7574 5f62 6174 6368 a900 720b  output_batch..r.
-00000170: 0000 00fa 542f 5573 6572 732f 6a65 6666  ....T/Users/jeff
-00000180: 6879 6b69 6e2f 7265 706f 732f 7472 6976  hykin/repos/triv
-00000190: 6961 6c2d 746f 7263 682d 746f 6f6c 732f  ial-torch-tools/
-000001a0: 6d61 696e 2f74 7269 7669 616c 5f74 6f72  main/trivial_tor
-000001b0: 6368 5f74 6f6f 6c73 2f63 6f6e 7465 6e74  ch_tools/content
-000001c0: 732f 6d69 7363 2e70 79da 1662 6174 6368  s/misc.py..batch
-000001d0: 5f69 6e70 7574 5f61 6e64 5f6f 7574 7075  _input_and_outpu
-000001e0: 7405 0000 0073 0800 0000 0001 0c01 1601  t....s..........
-000001f0: 0c01 720d 0000 0063 0300 0000 0000 0000  ..r....c........
-00000200: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
-00000210: 732a 0000 0064 0164 006c 006d 017d 0301  s*...d.d.l.m.}..
-00000220: 007c 03a0 027c 000b 007c 011b 0064 027c  .|...|...|...d.|
-00000230: 011b 00a1 027d 047c 047c 0283 0153 0029  .....}.|.|...S.)
-00000240: 034e 7201 0000 0067 0000 0000 0000 f03f  .Nr....g.......?
-00000250: 2903 5a16 746f 7263 6876 6973 696f 6e2e  ).Z.torchvision.
-00000260: 7472 616e 7366 6f72 6d73 da0a 7472 616e  transforms..tran
-00000270: 7366 6f72 6d73 5a09 4e6f 726d 616c 697a  sformsZ.Normaliz
-00000280: 6529 05da 046d 6561 6eda 0373 7464 da05  e)...mean..std..
-00000290: 696d 6167 6572 0e00 0000 5a0a 6e6f 726d  imager....Z.norm
-000002a0: 616c 697a 6572 720b 0000 0072 0b00 0000  alizerr....r....
-000002b0: 720c 0000 00da 0b75 6e6e 6f72 6d61 6c69  r......unnormali
-000002c0: 7a65 0b00 0000 7306 0000 0000 010c 0116  ze....s.........
-000002d0: 0172 1200 0000 6303 0000 0000 0000 0000  .r....c.........
-000002e0: 0000 0008 0000 000b 0000 0043 0000 0073  ...........C...s
-000002f0: 1c01 0000 6401 6402 6c00 6d01 7d03 0100  ....d.d.l.m.}...
-00000300: 7402 7c00 7403 8302 7222 7404 7c00 a005  t.|.t...r"t.|...
-00000310: a100 8301 7d00 7402 7c00 7404 8302 7236  ....}.t.|.t...r6
-00000320: 7406 6a07 7c00 8e00 7d00 7408 a009 6403  t.j.|...}.t...d.
-00000330: 7c01 9802 a101 7d04 7c02 6400 6b09 7256  |.....}.|.d.k.rV
-00000340: 7c04 a00a 7c02 a101 6e02 7c04 7d04 6700  |...|...n.|.}.g.
-00000350: 7d05 7408 a00b a100 8fac 0100 7a38 7c00  }.t.........z8|.
-00000360: 4400 5d2e 7d06 7402 7c06 7408 6a06 6a0c  D.].}.t.|.t.j.j.
-00000370: 6a0d 6a0e 8302 736e 7c06 a00f 7c04 a101  j.j...sn|...|...
-00000380: 7d04 7c05 a010 7c04 a011 a100 a101 0100  }.|...|.........
-00000390: 716e 5700 6e6c 0400 7412 6b0a 9001 720c  qnW.nl..t.k...r.
-000003a0: 0100 7d07 0100 7a4c 7c04 a00a 7c03 a101  ..}...zL|...|...
-000003b0: 7d04 7c00 4400 5d38 7d06 7402 7c06 7408  }.|.D.]8}.t.|.t.
-000003c0: 6a06 6a0c 6a0d 6a0e 8302 73c2 7c06 a00a  j.j.j.j...s.|...
-000003d0: 7c03 a101 7d06 7c06 a00f 7c04 a101 7d04  |...}.|...|...}.
-000003e0: 7c05 a010 7c04 a011 a100 a101 0100 71c2  |...|.........q.
-000003f0: 5700 3500 6400 7d07 7e07 5800 5900 6e02  W.5.d.}.~.X.Y.n.
-00000400: 5800 5700 3500 5100 5200 5800 7c05 5300  X.W.5.Q.R.X.|.S.
-00000410: 2904 4e72 0300 0000 2901 da0e 6465 6661  ).Nr....)...defa
-00000420: 756c 745f 6465 7669 6365 2901 7203 0000  ult_device).r...
-00000430: 0029 13da 0463 6f72 6572 1300 0000 da0a  .)...corer......
-00000440: 6973 696e 7374 616e 6365 7202 0000 00da  isinstancer.....
-00000450: 046c 6973 74da 0676 616c 7565 73da 026e  .list..values..n
-00000460: 6eda 0a53 6571 7565 6e74 6961 6cda 0574  n..Sequential..t
-00000470: 6f72 6368 da04 6f6e 6573 da02 746f da07  orch..ones..to..
-00000480: 6e6f 5f67 7261 64da 076d 6f64 756c 6573  no_grad..modules
-00000490: da04 6c6f 7373 da05 5f4c 6f73 73da 0766  ..loss.._Loss..f
-000004a0: 6f72 7761 7264 da06 6170 7065 6e64 da04  orward..append..
-000004b0: 7369 7a65 da09 4578 6365 7074 696f 6e29  size..Exception)
-000004c0: 08da 076e 6574 776f 726b da0b 696e 7075  ...network..inpu
-000004d0: 745f 7368 6170 65da 0664 6576 6963 6572  t_shape..devicer
-000004e0: 1300 0000 5a12 6e65 7572 6f6e 5f61 6374  ....Z.neuron_act
-000004f0: 6976 6174 696f 6e73 da05 7369 7a65 73da  ivations..sizes.
-00000500: 056c 6179 6572 da05 6572 726f 7272 0b00  .layer..errorr..
-00000510: 0000 720b 0000 0072 0c00 0000 da13 6c61  ..r....r......la
-00000520: 7965 725f 6f75 7470 7574 5f73 6861 7065  yer_output_shape
-00000530: 7311 0000 0073 2c00 0000 0001 0c02 0a01  s....s,.........
-00000540: 0c02 0a01 0a03 0e01 1601 0401 0a01 0201  ................
-00000550: 0802 1201 0a01 1401 1201 0a01 0802 1201  ................
-00000560: 0a01 0a01 2c02 722b 0000 0029 014e 2908  ....,.r+...).N).
-00000570: da0b 636f 6c6c 6563 7469 6f6e 7372 0200  ..collectionsr..
-00000580: 0000 721a 0000 00da 0874 6f72 6368 2e6e  ..r......torch.n
-00000590: 6e72 1800 0000 720d 0000 0072 1200 0000  nr....r....r....
-000005a0: 722b 0000 0072 0b00 0000 720b 0000 0072  r+...r....r....r
-000005b0: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
-000005c0: 6c65 3e01 0000 0073 0a00 0000 0c01 0801  le>....s........
-000005d0: 0c02 0806 0806                           ......
+00000050: 6404 6c05 6d06 5a06 0100 6405 6406 8400  d.l.m.Z...d.d...
+00000060: 5a07 6407 6408 8400 5a08 640f 6409 640a  Z.d.d...Z.d.d.d.
+00000070: 8401 5a09 640b 640c 8400 5a0a 4700 640d  ..Z.d.d...Z.G.d.
+00000080: 640e 8400 640e 8302 5a0b 6402 5300 2910  d...d...Z.d.S.).
+00000090: e900 0000 0029 01da 0b4f 7264 6572 6564  .....)...Ordered
+000000a0: 4469 6374 4ee9 0200 0000 2901 da0a 7375  DictN.....)...su
+000000b0: 7065 725f 6861 7368 6303 0000 0000 0000  per_hashc.......
+000000c0: 0000 0000 0007 0000 0005 0000 0063 0000  .............c..
+000000d0: 0073 4600 0000 6401 6402 6c00 6d01 7d03  .sF...d.d.l.m.}.
+000000e0: 0100 7402 7c03 7c00 7c02 8302 7c03 7c01  ..t.|.|.|...|.|.
+000000f0: 7c02 8302 8302 7d04 7c04 4400 5d1a 5c02  |.....}.|.D.].\.
+00000100: 7d05 7d06 7403 7c05 8301 7403 7c06 8301  }.}.t.|...t.|...
+00000110: 6602 5600 0100 7126 6400 5300 2903 4ee9  f.V...q&d.S.).N.
+00000120: 0100 0000 2901 da06 6275 6e64 6c65 2904  ....)...bundle).
+00000130: da08 6765 6e65 7269 6373 7206 0000 00da  ..genericsr.....
+00000140: 037a 6970 da09 746f 5f74 656e 736f 7229  .zip..to_tensor)
+00000150: 07da 0669 6e70 7574 73da 076f 7574 7075  ...inputs..outpu
+00000160: 7473 da0a 6261 7463 685f 7369 7a65 7206  ts..batch_sizer.
+00000170: 0000 005a 0762 6174 6368 6573 5a10 6561  ...Z.batchesZ.ea
+00000180: 6368 5f69 6e70 7574 5f62 6174 6368 5a11  ch_input_batchZ.
+00000190: 6561 6368 5f6f 7574 7075 745f 6261 7463  each_output_batc
+000001a0: 68a9 0072 0d00 0000 fa54 2f55 7365 7273  h..r.....T/Users
+000001b0: 2f6a 6566 6668 796b 696e 2f72 6570 6f73  /jeffhykin/repos
+000001c0: 2f74 7269 7669 616c 2d74 6f72 6368 2d74  /trivial-torch-t
+000001d0: 6f6f 6c73 2f6d 6169 6e2f 7472 6976 6961  ools/main/trivia
+000001e0: 6c5f 746f 7263 685f 746f 6f6c 732f 636f  l_torch_tools/co
+000001f0: 6e74 656e 7473 2f6d 6973 632e 7079 da16  ntents/misc.py..
+00000200: 6261 7463 685f 696e 7075 745f 616e 645f  batch_input_and_
+00000210: 6f75 7470 7574 0600 0000 7308 0000 0000  output....s.....
+00000220: 010c 0116 010c 0172 0f00 0000 6303 0000  .......r....c...
+00000230: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+00000240: 0043 0000 0073 2a00 0000 6401 6400 6c00  .C...s*...d.d.l.
+00000250: 6d01 7d03 0100 7c03 a002 7c00 0b00 7c01  m.}...|...|...|.
+00000260: 1b00 6402 7c01 1b00 a102 7d04 7c04 7c02  ..d.|.....}.|.|.
+00000270: 8301 5300 2903 4e72 0100 0000 6700 0000  ..S.).Nr....g...
+00000280: 0000 00f0 3f29 035a 1674 6f72 6368 7669  ....?).Z.torchvi
+00000290: 7369 6f6e 2e74 7261 6e73 666f 726d 73da  sion.transforms.
+000002a0: 0a74 7261 6e73 666f 726d 735a 094e 6f72  .transformsZ.Nor
+000002b0: 6d61 6c69 7a65 2905 da04 6d65 616e da03  malize)...mean..
+000002c0: 7374 64da 0569 6d61 6765 7210 0000 005a  std..imager....Z
+000002d0: 0a6e 6f72 6d61 6c69 7a65 7272 0d00 0000  .normalizerr....
+000002e0: 720d 0000 0072 0e00 0000 da0b 756e 6e6f  r....r......unno
+000002f0: 726d 616c 697a 650c 0000 0073 0600 0000  rmalize....s....
+00000300: 0001 0c01 1601 7214 0000 0063 0300 0000  ......r....c....
+00000310: 0000 0000 0000 0000 0800 0000 0b00 0000  ................
+00000320: 4300 0000 731c 0100 0064 0164 026c 006d  C...s....d.d.l.m
+00000330: 017d 0301 0074 027c 0074 0383 0272 2274  .}...t.|.t...r"t
+00000340: 047c 00a0 05a1 0083 017d 0074 027c 0074  .|.......}.t.|.t
+00000350: 0483 0272 3674 066a 077c 008e 007d 0074  ...r6t.j.|...}.t
+00000360: 08a0 0964 037c 0198 02a1 017d 047c 0264  ...d.|.....}.|.d
+00000370: 006b 0972 567c 04a0 0a7c 02a1 016e 027c  .k.rV|...|...n.|
+00000380: 047d 0467 007d 0574 08a0 0ba1 008f ac01  .}.g.}.t........
+00000390: 007a 387c 0044 005d 2e7d 0674 027c 0674  .z8|.D.].}.t.|.t
+000003a0: 086a 066a 0c6a 0d6a 0e83 0273 6e7c 06a0  .j.j.j.j...sn|..
+000003b0: 0f7c 04a1 017d 047c 05a0 107c 04a0 11a1  .|...}.|...|....
+000003c0: 00a1 0101 0071 6e57 006e 6c04 0074 126b  .....qnW.nl..t.k
+000003d0: 0a90 0172 0c01 007d 0701 007a 4c7c 04a0  ...r...}...zL|..
+000003e0: 0a7c 03a1 017d 047c 0044 005d 387d 0674  .|...}.|.D.]8}.t
+000003f0: 027c 0674 086a 066a 0c6a 0d6a 0e83 0273  .|.t.j.j.j.j...s
+00000400: c27c 06a0 0a7c 03a1 017d 067c 06a0 0f7c  .|...|...}.|...|
+00000410: 04a1 017d 047c 05a0 107c 04a0 11a1 00a1  ...}.|...|......
+00000420: 0101 0071 c257 0035 0064 007d 077e 0758  ...q.W.5.d.}.~.X
+00000430: 0059 006e 0258 0057 0035 0051 0052 0058  .Y.n.X.W.5.Q.R.X
+00000440: 007c 0553 0029 044e 7205 0000 0029 01da  .|.S.).Nr....)..
+00000450: 0e64 6566 6175 6c74 5f64 6576 6963 6529  .default_device)
+00000460: 0172 0500 0000 2913 da04 636f 7265 7215  .r....)...corer.
+00000470: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
+00000480: 0200 0000 da04 6c69 7374 da06 7661 6c75  ......list..valu
+00000490: 6573 da02 6e6e da0a 5365 7175 656e 7469  es..nn..Sequenti
+000004a0: 616c da05 746f 7263 68da 046f 6e65 73da  al..torch..ones.
+000004b0: 0274 6fda 076e 6f5f 6772 6164 da07 6d6f  .to..no_grad..mo
+000004c0: 6475 6c65 73da 046c 6f73 73da 055f 4c6f  dules..loss.._Lo
+000004d0: 7373 da07 666f 7277 6172 64da 0661 7070  ss..forward..app
+000004e0: 656e 64da 0473 697a 65da 0945 7863 6570  end..size..Excep
+000004f0: 7469 6f6e 2908 da07 6e65 7477 6f72 6bda  tion)...network.
+00000500: 0b69 6e70 7574 5f73 6861 7065 da06 6465  .input_shape..de
+00000510: 7669 6365 7215 0000 005a 126e 6575 726f  vicer....Z.neuro
+00000520: 6e5f 6163 7469 7661 7469 6f6e 73da 0573  n_activations..s
+00000530: 697a 6573 da05 6c61 7965 72da 0565 7272  izes..layer..err
+00000540: 6f72 720d 0000 0072 0d00 0000 720e 0000  orr....r....r...
+00000550: 00da 136c 6179 6572 5f6f 7574 7075 745f  ...layer_output_
+00000560: 7368 6170 6573 1200 0000 732c 0000 0000  shapes....s,....
+00000570: 010c 020a 010c 020a 010a 030e 0116 0104  ................
+00000580: 010a 0102 0108 0212 010a 0114 0112 010a  ................
+00000590: 0108 0212 010a 010a 012c 0272 2d00 0000  .........,.r-...
+000005a0: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+000005b0: 0004 0000 0043 0000 0073 4000 0000 7c00  .....C...s@...|.
+000005c0: a000 a100 7d01 7401 8300 7d02 6401 7d03  ....}.t...}.d.}.
+000005d0: 6402 7d04 7402 7c00 a000 a100 8301 4400  d.}.t.|.......D.
+000005e0: 5d18 5c02 7d05 7d03 7c03 7c04 7c05 1300  ].\.}.}.|.|.|...
+000005f0: 7c03 1400 3700 7d03 7122 7c03 5300 2903  |...7.}.q"|.S.).
+00000600: 4e72 0100 0000 e900 0100 0029 03da 0665  Nr.........)...e
+00000610: 6e63 6f64 65da 0373 6574 da09 656e 756d  ncode..set..enum
+00000620: 6572 6174 6529 06da 0673 7472 696e 67da  erate)...string.
+00000630: 086f 7269 6769 6e61 6c5a 0d75 7365 645f  .originalZ.used_
+00000640: 696e 6469 6369 6573 da06 6e75 6d62 6572  indicies..number
+00000650: da04 6261 7365 da05 696e 6465 7872 0d00  ..base..indexr..
+00000660: 0000 720d 0000 0072 0e00 0000 da16 5f73  ..r....r......_s
+00000670: 7472 696e 675f 6861 7368 5f74 6f5f 6e75  tring_hash_to_nu
+00000680: 6d62 6572 3100 0000 730e 0000 0000 0108  mber1...s.......
+00000690: 0106 0104 0104 0114 0112 0172 3700 0000  ...........r7...
+000006a0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000006b0: 0002 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
+000006c0: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+000006d0: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
+000006e0: 5a06 6408 5300 2909 da15 4465 7465 726d  Z.d.S.)...Determ
+000006f0: 696e 6973 7469 6354 6f72 6368 526e 676c  inisticTorchRngl
+00000700: 0500 0000 ff7f ff7f ff7f ff7f 0f00 6301  ..............c.
+00000710: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000720: 0000 004f 0000 0073 1800 0000 7400 7401  ...O...s....t.t.
+00000730: 7c01 8301 8301 7402 6a03 1600 7c00 5f04  |.....t.j...|._.
+00000740: 6400 5300 a901 4e29 0572 3700 0000 7204  d.S...N).r7...r.
+00000750: 0000 0072 3800 0000 da15 6d61 785f 7079  ...r8.....max_py
+00000760: 746f 7263 685f 7365 6564 5f73 697a 65da  torch_seed_size.
+00000770: 0d74 656d 705f 726e 675f 7365 6564 2903  .temp_rng_seed).
+00000780: da04 7365 6c66 da04 6172 6773 da06 6b77  ..self..args..kw
+00000790: 6172 6773 720d 0000 0072 0d00 0000 720e  argsr....r....r.
+000007a0: 0000 00da 085f 5f69 6e69 745f 5f3c 0000  .....__init__<..
+000007b0: 0073 0200 0000 0001 7a1e 4465 7465 726d  .s......z.Determ
+000007c0: 696e 6973 7469 6354 6f72 6368 526e 672e  inisticTorchRng.
+000007d0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+000007e0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000007f0: 0073 1c00 0000 7400 6a01 a002 a100 7c00  .s....t.j.....|.
+00000800: 5f03 7400 a004 7c00 6a05 a101 0100 6400  _.t...|.j.....d.
+00000810: 5300 7239 0000 0029 0672 1c00 0000 da06  S.r9...).r......
+00000820: 7261 6e64 6f6d da0d 6765 745f 726e 675f  random..get_rng_
+00000830: 7374 6174 65da 126f 7269 6769 6e61 6c5f  state..original_
+00000840: 726e 675f 7374 6174 65da 0b6d 616e 7561  rng_state..manua
+00000850: 6c5f 7365 6564 723b 0000 0029 0172 3c00  l_seedr;...).r<.
+00000860: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000870: 00da 095f 5f65 6e74 6572 5f5f 3f00 0000  ...__enter__?...
+00000880: 7306 0000 0000 010c 010c 017a 1f44 6574  s..........z.Det
+00000890: 6572 6d69 6e69 7374 6963 546f 7263 6852  erministicTorchR
+000008a0: 6e67 2e5f 5f65 6e74 6572 5f5f 6304 0000  ng.__enter__c...
+000008b0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+000008c0: 0043 0000 0073 1e00 0000 7400 6a01 a002  .C...s....t.j...
+000008d0: 7c00 6a03 a101 0100 7c02 6400 6b09 721a  |.j.....|.d.k.r.
+000008e0: 7c02 8201 6400 5300 7239 0000 0029 0472  |...d.S.r9...).r
+000008f0: 1c00 0000 7240 0000 00da 0d73 6574 5f72  ....r@.....set_r
+00000900: 6e67 5f73 7461 7465 7242 0000 0029 0472  ng_staterB...).r
+00000910: 3c00 0000 da01 5f72 2c00 0000 da09 7472  <....._r,.....tr
+00000920: 6163 6562 6163 6b72 0d00 0000 720d 0000  acebackr....r...
+00000930: 0072 0e00 0000 da08 5f5f 6578 6974 5f5f  .r......__exit__
+00000940: 4400 0000 7306 0000 0000 020e 0108 027a  D...s..........z
+00000950: 1e44 6574 6572 6d69 6e69 7374 6963 546f  .DeterministicTo
+00000960: 7263 6852 6e67 2e5f 5f65 7869 745f 5f4e  rchRng.__exit__N
+00000970: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000980: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000990: 6e61 6d65 5f5f 723a 0000 0072 3f00 0000  name__r:...r?...
+000009a0: 7244 0000 0072 4800 0000 720d 0000 0072  rD...rH...r....r
+000009b0: 0d00 0000 720d 0000 0072 0e00 0000 7238  ....r....r....r8
+000009c0: 0000 003a 0000 0073 0800 0000 0801 0401  ...:...s........
+000009d0: 0803 0805 7238 0000 0029 014e 290c da0b  ....r8...).N)...
+000009e0: 636f 6c6c 6563 7469 6f6e 7372 0200 0000  collectionsr....
+000009f0: 721c 0000 00da 0874 6f72 6368 2e6e 6e72  r......torch.nnr
+00000a00: 1a00 0000 5a1b 5f5f 6465 7065 6e64 656e  ....Z.__dependen
+00000a10: 6369 6573 5f5f 2e73 7570 6572 5f68 6173  cies__.super_has
+00000a20: 6872 0400 0000 720f 0000 0072 1400 0000  hr....r....r....
+00000a30: 722d 0000 0072 3700 0000 7238 0000 0072  r-...r7...r8...r
+00000a40: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00000a50: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000a60: 0073 1000 0000 0c01 0801 0c01 0c02 0806  .s..............
+00000a70: 0806 0a1f 0809                           ......
```

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/model.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/model.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/__pycache__/one_hots.cpython-38.pyc` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/__pycache__/one_hots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/core.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/core.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/generics.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/generics.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/image.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/image.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/main.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/main.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/model.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/model.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools/contents/one_hots.py` & `trivial_torch_tools-0.6.1/trivial_torch_tools/contents/one_hots.py`

 * *Files identical despite different names*

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/PKG-INFO` & `trivial_torch_tools-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: trivial-torch-tools
-Version: 0.6.0
+Name: trivial_torch_tools
+Version: 0.6.1
 Summary: Decorators for reducing pytorch boilerplate
 Home-page: https://github.com/jeff-hykin/trivial-torch-tools.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `trivial_torch_tools-0.6.0/trivial_torch_tools.egg-info/SOURCES.txt` & `trivial_torch_tools-0.6.1/trivial_torch_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

