# Comparing `tmp/oxenai-0.1.0.tar.gz` & `tmp/oxenai-0.1.1.tar.gz`

## Comparing `oxenai-0.1.0.tar` & `oxenai-0.1.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 oxenai-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-24 18:10:45.000000 oxenai-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-24 18:10:45.000000 oxenai-0.1.0/.gitignore
--rw-r--r--   0      501       20      984 2023-05-11 16:11:21.000000 oxenai-0.1.0/README.md
--rw-r--r--   0      501       20      638 2023-05-16 20:02:04.000000 oxenai-0.1.0/docs/Makefile
--rw-r--r--   0      501       20      804 2023-05-16 20:02:04.000000 oxenai-0.1.0/docs/make.bat
--rw-r--r--   0      501       20     1348 2023-05-18 04:48:44.000000 oxenai-0.1.0/docs/source/conf.py
--rw-r--r--   0      501       20      435 2023-05-17 22:27:30.000000 oxenai-0.1.0/docs/source/getting_started/commands.md
--rw-r--r--   0      501       20     2148 2023-05-18 04:14:06.000000 oxenai-0.1.0/docs/source/getting_started/installation.md
--rw-r--r--   0      501       20     1041 2023-05-18 03:41:56.000000 oxenai-0.1.0/docs/source/getting_started/python.md
--rw-r--r--   0      501       20       18 2023-05-17 00:07:17.000000 oxenai-0.1.0/docs/source/getting_started/tutorials.md
--rw-r--r--   0      501       20      753 2023-05-18 04:21:40.000000 oxenai-0.1.0/docs/source/index.rst
--rw-r--r--   0      501       20       69 2023-05-18 03:59:38.000000 oxenai-0.1.0/docs/source/references/python/local_repo.rst
--rw-r--r--   0      501       20       68 2023-05-18 04:14:40.000000 oxenai-0.1.0/docs/source/references/python/remote_repo.rst
--rw-r--r--   0      501       20      235 2023-05-18 04:22:39.000000 oxenai-0.1.0/docs/source/references/rust.md
--rw-r--r--   0      501       20      451 2023-05-18 05:03:17.000000 oxenai-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      560 2023-05-18 04:28:27.000000 oxenai-0.1.0/python/oxen/__init__.py
--rw-r--r--   0      501       20      656 2023-05-12 22:34:40.000000 oxenai-0.1.0/python/oxen/dag.py
--rw-r--r--   0      501       20     5995 2023-05-12 22:03:31.000000 oxenai-0.1.0/python/oxen/dataset.py
--rw-r--r--   0      501       20     1378 2023-05-11 01:03:21.000000 oxenai-0.1.0/python/oxen/features.py
--rw-r--r--   0      501       20      181 2023-05-12 22:50:15.000000 oxenai-0.1.0/python/oxen/loaders/__init__.py
--rw-r--r--   0      501       20     1057 2023-05-12 22:37:03.000000 oxenai-0.1.0/python/oxen/loaders/chat.py
--rw-r--r--   0      501       20        0 2023-05-12 02:11:27.000000 oxenai-0.1.0/python/oxen/loaders/image_classification.py
--rw-r--r--   0      501       20      802 2023-05-12 22:56:45.000000 oxenai-0.1.0/python/oxen/loaders/regression.py
--rw-r--r--   0      501       20     3732 2023-05-18 04:48:44.000000 oxenai-0.1.0/python/oxen/local_repo.py
--rw-r--r--   0      501       20     1498 2023-05-12 22:34:23.000000 oxenai-0.1.0/python/oxen/op.py
--rw-r--r--   0      501       20      390 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/__init__.py
--rw-r--r--   0      501       20      207 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/concat_series.py
--rw-r--r--   0      501       20      203 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/extract_col.py
--rw-r--r--   0      501       20      214 2023-05-12 22:34:50.000000 oxenai-0.1.0/python/oxen/ops/identity.py
--rw-r--r--   0      501       20      224 2023-05-12 22:35:42.000000 oxenai-0.1.0/python/oxen/ops/read_df.py
--rw-r--r--   0      501       20      235 2023-05-12 22:35:42.000000 oxenai-0.1.0/python/oxen/ops/read_text.py
--rw-r--r--   0      501       20      354 2023-05-12 22:33:21.000000 oxenai-0.1.0/python/oxen/ops/str_col_template.py
--rw-r--r--   0      501       20     5494 2023-05-18 04:48:44.000000 oxenai-0.1.0/python/oxen/remote_repo.py
--rw-r--r--   0      501       20        0 2023-04-27 17:45:52.000000 oxenai-0.1.0/python/oxen/util/__init__.py
--rw-r--r--   0      501       20     1500 2023-05-18 04:26:23.000000 oxenai-0.1.0/python/oxen/util/fs.py
--rw-r--r--   0      501       20      144 2023-05-18 04:12:52.000000 oxenai-0.1.0/requirements.txt
--rw-r--r--   0      501       20      370 2023-04-26 18:47:19.000000 oxenai-0.1.0/src/error.rs
--rw-r--r--   0      501       20     1726 2023-05-18 04:50:52.000000 oxenai-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      718 2023-05-18 04:53:34.000000 oxenai-0.1.0/src/py_branch.rs
--rw-r--r--   0      501       20      291 2023-04-26 18:47:19.000000 oxenai-0.1.0/src/py_commit.rs
--rw-r--r--   0      501       20      474 2023-05-05 03:46:35.000000 oxenai-0.1.0/src/py_dataset.rs
--rw-r--r--   0      501       20     3875 2023-05-18 04:51:00.000000 oxenai-0.1.0/src/py_local_repo.rs
--rw-r--r--   0      501       20     8111 2023-05-18 04:50:52.000000 oxenai-0.1.0/src/py_remote_repo.rs
--rw-r--r--   0      501       20     1572 2023-05-17 00:12:30.000000 oxenai-0.1.0/src/py_staged_data.rs
--rw-r--r--   0      501       20      538 2023-05-17 00:12:30.000000 oxenai-0.1.0/src/util.rs
--rw-r--r--   0      501       20      345 2023-05-18 02:53:28.000000 oxenai-0.1.0/test.py
--rw-r--r--   0      501       20        0 2023-04-26 19:43:28.000000 oxenai-0.1.0/tests/__init__.py
--rw-r--r--   0      501       20     3474 2023-05-18 04:26:36.000000 oxenai-0.1.0/tests/conftest.py
--rw-r--r--   0      501       20      114 2023-04-25 22:04:20.000000 oxenai-0.1.0/tests/data/CelebA/annotations/test.csv
--rw-r--r--   0      501       20      139 2023-04-25 22:04:25.000000 oxenai-0.1.0/tests/data/CelebA/annotations/train.csv
--rw-r--r--   0      501       20    11440 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/1.jpg
--rw-r--r--   0      501       20     7448 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/2.jpg
--rw-r--r--   0      501       20     4253 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/3.jpg
--rw-r--r--   0      501       20    10747 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/4.jpg
--rw-r--r--   0      501       20     6351 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/5.jpg
--rw-r--r--   0      501       20     8073 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/6.jpg
--rw-r--r--   0      501       20     8203 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/7.jpg
--rw-r--r--   0      501       20     7725 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/8.jpg
--rw-r--r--   0      501       20     8641 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/9.jpg
--rw-r--r--   0      501       20      337 2023-05-12 22:23:52.000000 oxenai-0.1.0/tests/data/ChatBot/examples.tsv
--rw-r--r--   0      501       20       88 2023-05-12 22:31:17.000000 oxenai-0.1.0/tests/data/ChatBot/prompt.txt
--rw-r--r--   0      501       20      148 2023-05-12 22:42:34.000000 oxenai-0.1.0/tests/data/HousePrices/prices.csv
--rw-r--r--   0      501       20      477 2023-05-18 04:26:41.000000 oxenai-0.1.0/tests/test_add.py
--rw-r--r--   0      501       20      363 2023-05-12 22:35:42.000000 oxenai-0.1.0/tests/test_chat_loader.py
--rw-r--r--   0      501       20     1299 2023-05-18 04:46:14.000000 oxenai-0.1.0/tests/test_checkout.py
--rw-r--r--   0      501       20      716 2023-05-18 04:26:46.000000 oxenai-0.1.0/tests/test_clone.py
--rw-r--r--   0      501       20      850 2023-04-29 18:40:43.000000 oxenai-0.1.0/tests/test_commit.py
--rw-r--r--   0      501       20     2444 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_dataloader_pytorch.py
--rw-r--r--   0      501       20     1506 2023-05-18 04:48:44.000000 oxenai-0.1.0/tests/test_dataset.py
--rw-r--r--   0      501       20      338 2023-05-18 04:26:51.000000 oxenai-0.1.0/tests/test_init.py
--rw-r--r--   0      501       20      440 2023-04-29 22:00:54.000000 oxenai-0.1.0/tests/test_push.py
--rw-r--r--   0      501       20      916 2023-05-18 04:26:56.000000 oxenai-0.1.0/tests/test_push_pull.py
--rw-r--r--   0      501       20      488 2023-05-12 22:56:45.000000 oxenai-0.1.0/tests/test_regression_loader.py
--rw-r--r--   0      501       20      828 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_add.py
--rw-r--r--   0      501       20      560 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_branch.py
--rw-r--r--   0      501       20      538 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_remote_checkout.py
--rw-r--r--   0      501       20      685 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_commit.py
--rw-r--r--   0      501       20     1473 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_remote_df_add.py
--rw-r--r--   0      501       20      530 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_list.py
--rw-r--r--   0      501       20      657 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_remove.py
--rw-r--r--   0      501       20      114 2023-04-27 16:40:57.000000 oxenai-0.1.0/tests/test_remote_repo.py
--rw-r--r--   0      501       20      636 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_status.py
--rw-r--r--   0      501       20      259 2023-05-18 04:27:00.000000 oxenai-0.1.0/tests/test_status.py
--rw-r--r--   0      501       20   109486 2023-05-17 21:25:52.000000 oxenai-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 oxenai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 oxenai-0.1.1/Cargo.toml
+-rw-rw-r--   0     1000     1000     2809 2023-05-18 06:17:53.000000 oxenai-0.1.1/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      685 2023-05-18 06:17:53.000000 oxenai-0.1.1/.gitignore
+-rw-rw-r--   0     1000     1000      984 2023-05-18 06:17:53.000000 oxenai-0.1.1/README.md
+-rw-rw-r--   0     1000     1000      638 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/Makefile
+-rw-rw-r--   0     1000     1000      804 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/make.bat
+-rw-rw-r--   0     1000     1000      117 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/requirements.txt
+-rw-rw-r--   0     1000     1000     1348 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/conf.py
+-rw-rw-r--   0     1000     1000      435 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/getting_started/commands.md
+-rw-rw-r--   0     1000     1000     2148 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/getting_started/installation.md
+-rw-rw-r--   0     1000     1000     1041 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/getting_started/python.md
+-rw-rw-r--   0     1000     1000       18 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/getting_started/tutorials.md
+-rw-rw-r--   0     1000     1000      753 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/index.rst
+-rw-rw-r--   0     1000     1000       69 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/references/python/local_repo.rst
+-rw-rw-r--   0     1000     1000       68 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/references/python/remote_repo.rst
+-rw-rw-r--   0     1000     1000      235 2023-05-18 06:17:53.000000 oxenai-0.1.1/docs/source/references/rust.md
+-rw-rw-r--   0     1000     1000      451 2023-05-18 06:37:00.000000 oxenai-0.1.1/pyproject.toml
+-rw-rw-r--   0     1000     1000      560 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/__init__.py
+-rw-rw-r--   0     1000     1000      656 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/dag.py
+-rw-rw-r--   0     1000     1000     5995 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/dataset.py
+-rw-rw-r--   0     1000     1000     1378 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/features.py
+-rw-rw-r--   0     1000     1000      181 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/loaders/__init__.py
+-rw-rw-r--   0     1000     1000     1057 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/loaders/chat.py
+-rw-rw-r--   0     1000     1000        0 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/loaders/image_classification.py
+-rw-rw-r--   0     1000     1000      802 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/loaders/regression.py
+-rw-rw-r--   0     1000     1000     3732 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/local_repo.py
+-rw-rw-r--   0     1000     1000     1498 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/op.py
+-rw-rw-r--   0     1000     1000      390 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/__init__.py
+-rw-rw-r--   0     1000     1000      207 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/concat_series.py
+-rw-rw-r--   0     1000     1000      203 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/extract_col.py
+-rw-rw-r--   0     1000     1000      214 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/identity.py
+-rw-rw-r--   0     1000     1000      224 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/read_df.py
+-rw-rw-r--   0     1000     1000      235 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/read_text.py
+-rw-rw-r--   0     1000     1000      354 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/ops/str_col_template.py
+-rw-rw-r--   0     1000     1000     5494 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/remote_repo.py
+-rw-rw-r--   0     1000     1000        0 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/util/__init__.py
+-rw-rw-r--   0     1000     1000     1500 2023-05-18 06:17:53.000000 oxenai-0.1.1/python/oxen/util/fs.py
+-rw-rw-r--   0     1000     1000       82 2023-05-18 06:17:53.000000 oxenai-0.1.1/requirements.txt
+-rw-rw-r--   0     1000     1000      370 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/error.rs
+-rw-rw-r--   0     1000     1000     1726 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/lib.rs
+-rw-rw-r--   0     1000     1000      718 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_branch.rs
+-rw-rw-r--   0     1000     1000      291 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_commit.rs
+-rw-rw-r--   0     1000     1000      474 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_dataset.rs
+-rw-rw-r--   0     1000     1000     3875 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_local_repo.rs
+-rw-rw-r--   0     1000     1000     8111 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_remote_repo.rs
+-rw-rw-r--   0     1000     1000     1572 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/py_staged_data.rs
+-rw-rw-r--   0     1000     1000      538 2023-05-18 06:17:53.000000 oxenai-0.1.1/src/util.rs
+-rw-rw-r--   0     1000     1000      345 2023-05-18 06:17:53.000000 oxenai-0.1.1/test.py
+-rw-rw-r--   0     1000     1000        0 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/__init__.py
+-rw-rw-r--   0     1000     1000     3474 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/conftest.py
+-rw-rw-r--   0     1000     1000      114 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/annotations/test.csv
+-rw-rw-r--   0     1000     1000      139 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/annotations/train.csv
+-rw-rw-r--   0     1000     1000    11440 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/1.jpg
+-rw-rw-r--   0     1000     1000     7448 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/2.jpg
+-rw-rw-r--   0     1000     1000     4253 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/3.jpg
+-rw-rw-r--   0     1000     1000    10747 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/4.jpg
+-rw-rw-r--   0     1000     1000     6351 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/5.jpg
+-rw-rw-r--   0     1000     1000     8073 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/6.jpg
+-rw-rw-r--   0     1000     1000     8203 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/7.jpg
+-rw-rw-r--   0     1000     1000     7725 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/8.jpg
+-rw-rw-r--   0     1000     1000     8641 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/CelebA/images/9.jpg
+-rw-rw-r--   0     1000     1000      337 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/ChatBot/examples.tsv
+-rw-rw-r--   0     1000     1000       88 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/ChatBot/prompt.txt
+-rw-rw-r--   0     1000     1000      148 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/data/HousePrices/prices.csv
+-rw-rw-r--   0     1000     1000      477 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_add.py
+-rw-rw-r--   0     1000     1000      363 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_chat_loader.py
+-rw-rw-r--   0     1000     1000     1299 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_checkout.py
+-rw-rw-r--   0     1000     1000      716 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_clone.py
+-rw-rw-r--   0     1000     1000      850 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_commit.py
+-rw-rw-r--   0     1000     1000     2444 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_dataloader_pytorch.py
+-rw-rw-r--   0     1000     1000     1506 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_dataset.py
+-rw-rw-r--   0     1000     1000      338 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_init.py
+-rw-rw-r--   0     1000     1000      440 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_push.py
+-rw-rw-r--   0     1000     1000      916 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_push_pull.py
+-rw-rw-r--   0     1000     1000      488 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_regression_loader.py
+-rw-rw-r--   0     1000     1000      828 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_add.py
+-rw-rw-r--   0     1000     1000      560 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_branch.py
+-rw-rw-r--   0     1000     1000      538 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_checkout.py
+-rw-rw-r--   0     1000     1000      685 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_commit.py
+-rw-rw-r--   0     1000     1000     1473 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_df_add.py
+-rw-rw-r--   0     1000     1000      530 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_list.py
+-rw-rw-r--   0     1000     1000      657 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_remove.py
+-rw-rw-r--   0     1000     1000      114 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_repo.py
+-rw-rw-r--   0     1000     1000      636 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_remote_status.py
+-rw-rw-r--   0     1000     1000      259 2023-05-18 06:17:53.000000 oxenai-0.1.1/tests/test_status.py
+-rw-rw-r--   0     1000     1000   109486 2023-05-18 06:56:50.000000 oxenai-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 oxenai-0.1.1/PKG-INFO
```

### Comparing `oxenai-0.1.0/.github/workflows/CI.yml` & `oxenai-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/.gitignore` & `oxenai-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/README.md` & `oxenai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/Makefile` & `oxenai-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/make.bat` & `oxenai-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/conf.py` & `oxenai-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/getting_started/installation.md` & `oxenai-0.1.1/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/getting_started/python.md` & `oxenai-0.1.1/docs/source/getting_started/python.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/index.rst` & `oxenai-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/__init__.py` & `oxenai-0.1.1/python/oxen/__init__.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/dag.py` & `oxenai-0.1.1/python/oxen/dag.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/dataset.py` & `oxenai-0.1.1/python/oxen/dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/features.py` & `oxenai-0.1.1/python/oxen/features.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/loaders/chat.py` & `oxenai-0.1.1/python/oxen/loaders/chat.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/loaders/regression.py` & `oxenai-0.1.1/python/oxen/loaders/regression.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/local_repo.py` & `oxenai-0.1.1/python/oxen/local_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/op.py` & `oxenai-0.1.1/python/oxen/op.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/remote_repo.py` & `oxenai-0.1.1/python/oxen/remote_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/util/fs.py` & `oxenai-0.1.1/python/oxen/util/fs.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/lib.rs` & `oxenai-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_branch.rs` & `oxenai-0.1.1/src/py_branch.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_local_repo.rs` & `oxenai-0.1.1/src/py_local_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_remote_repo.rs` & `oxenai-0.1.1/src/py_remote_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_staged_data.rs` & `oxenai-0.1.1/src/py_staged_data.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/util.rs` & `oxenai-0.1.1/src/util.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/conftest.py` & `oxenai-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/1.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/1.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/2.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/2.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/3.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/3.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/4.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/4.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/5.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/5.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/6.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/6.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/7.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/7.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/8.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/8.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/9.jpg` & `oxenai-0.1.1/tests/data/CelebA/images/9.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_checkout.py` & `oxenai-0.1.1/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_clone.py` & `oxenai-0.1.1/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_commit.py` & `oxenai-0.1.1/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_dataloader_pytorch.py` & `oxenai-0.1.1/tests/test_dataloader_pytorch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_dataset.py` & `oxenai-0.1.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_push_pull.py` & `oxenai-0.1.1/tests/test_push_pull.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_add.py` & `oxenai-0.1.1/tests/test_remote_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_branch.py` & `oxenai-0.1.1/tests/test_remote_branch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_checkout.py` & `oxenai-0.1.1/tests/test_remote_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_commit.py` & `oxenai-0.1.1/tests/test_remote_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_df_add.py` & `oxenai-0.1.1/tests/test_remote_df_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_list.py` & `oxenai-0.1.1/tests/test_remote_list.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_remove.py` & `oxenai-0.1.1/tests/test_remote_remove.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_status.py` & `oxenai-0.1.1/tests/test_remote_status.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/Cargo.lock` & `oxenai-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2461,15 +2461,15 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "oxen"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "liboxen",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "pyo3-polars",
```

### Comparing `oxenai-0.1.0/PKG-INFO` & `oxenai-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxenai
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Data version control for machine learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

