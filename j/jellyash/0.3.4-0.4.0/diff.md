# Comparing `tmp/jellyash-0.3.4.tar.gz` & `tmp/jellyash-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyash-0.3.4.tar", last modified: Sun Apr 30 08:37:35 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jellyash-0.3.4.tar` & `jellyash-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,307 @@
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1080 2023-01-31 23:22:28.000000 jellyash-0.3.4/LICENSE
--rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-04-30 08:37:35.303136 jellyash-0.3.4/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      693 2023-02-06 00:46:32.000000 jellyash-0.3.4/README.md
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/jellyash/
--rw-rw-r--   0 steven    (1000) steven    (1000)       22 2023-04-30 08:26:35.000000 jellyash-0.3.4/jellyash/__init__.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     1264 2023-04-30 07:51:28.000000 jellyash-0.3.4/jellyash/bundle.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     1451 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/client.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      813 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/duration.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      556 2023-04-30 08:30:37.000000 jellyash-0.3.4/jellyash/nextup.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      494 2023-04-30 08:26:35.000000 jellyash-0.3.4/jellyash/series.py
--rw-rw-r--   0 steven    (1000) steven    (1000)      906 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/token.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     1281 2023-04-30 08:22:47.000000 jellyash-0.3.4/jellyash/unwatched.py
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/jellyash.egg-info/
--rw-rw-r--   0 steven    (1000) steven    (1000)     1970 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      426 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/SOURCES.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/dependency_links.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)      206 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/entry_points.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)       72 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/requires.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        9 2023-04-30 08:37:35.000000 jellyash-0.3.4/jellyash.egg-info/top_level.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)      593 2023-04-30 08:22:47.000000 jellyash-0.3.4/pyproject.toml
--rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-04-30 08:37:35.303136 jellyash-0.3.4/setup.cfg
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-30 08:37:35.303136 jellyash-0.3.4/tests/
--rw-rw-r--   0 steven    (1000) steven    (1000)      666 2023-04-30 07:50:08.000000 jellyash-0.3.4/tests/test_bundle.py
--rw-rw-r--   0 steven    (1000) steven    (1000)     2463 2023-04-30 07:52:18.000000 jellyash-0.3.4/tests/test_client.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jellyash-0.4.0/tox.ini
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0   177663 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    52396 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   170956 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0   111332 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_operator.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_operator.meta.json
+-rw-r--r--   0        0        0    23358 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0   149720 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/argparse.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/argparse.meta.json
+-rw-r--r--   0        0        0    60683 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1054946 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   123324 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   104156 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    57608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    40359 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dis.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dis.meta.json
+-rw-r--r--   0        0        0    61016 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/getpass.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/getpass.meta.json
+-rw-r--r--   0        0        0   339721 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/inspect.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/inspect.meta.json
+-rw-r--r--   0        0        0    85344 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0    28774 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    78978 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/opcode.data.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/opcode.meta.json
+-rw-r--r--   0        0        0    46568 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/operator.data.json
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/operator.meta.json
+-rw-r--r--   0        0        0    88250 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    44389 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    34948 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/platform.data.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/platform.meta.json
+-rw-r--r--   0        0        0    75204 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0   167171 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    14127 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    28009 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    49438 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   157890 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   140040 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   228226 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   417108 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73945 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33582 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/uuid.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/uuid.meta.json
+-rw-r--r--   0        0        0    89061 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   407995 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   128990 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25069 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    79277 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    30853 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70171 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64567 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    90273 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11931 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/jellyash/__init__.data.json
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/jellyash/__init__.meta.json
+-rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/__init__.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/__init__.meta.json
+-rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/decoder.data.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/decoder.meta.json
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/encoder.data.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/encoder.meta.json
+-rw-r--r--   0        0        0   350174 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1161349852a407df
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/11fe4e56a1a0998f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/12eed7b0df0436e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/139b0884db11e1e8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/143665f5d7894aaf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1463469ef69bf78e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/16cb39ad3861193e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1919e19d29d7caa0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/19b2b937d1a7ab43
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1d70761d4d816b30
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1dd3bcd5629284a8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1efcba8af52f7427
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1f2e9a081c8f8f99
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1fd53c5cd1e0cb59
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/208903efda15df61
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/20e749519f49b18e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2673cfaf4403e190
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/278d08fe3071dc9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/27e6962f095a9afa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2ce46804cb25434d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2dc240553e4605e6
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2f2e286f4d93fe12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2f8d01deff758aca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/344663dba662e101
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/369321b91d77fd86
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3a082fd391280242
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3b0f5f3f4ca662f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3c6eb77fc9daaf4b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3ec68bfe2bd02760
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/411c11eda0979215
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/41528c30d4c7c82e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/41e7b66b53d2a24c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/422079b659902906
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/426cd6790b31a273
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/43e057b3dcc43e96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/49a5af4645b42506
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/4c9e958d28374767
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5001be39813f2835
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5017eb9f3edaf502
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/521750f423c285e6
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/52b08a05f3469c2
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/53abdaef3ad7e08e
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/562cf0d217c2e526
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/563b1ff8799d6d2f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/58136763caf87fdc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/581c717c582cac6d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/59fa0f38996b9d60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5aa88ef31443a878
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6201111bf7b60a76
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/625181274b029d67
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/62b82a00fa7de2b5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/62ed103883955520
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/655a1e70b9bf2246
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/669a75b0670c256b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/68382171887c4592
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6a5d72074f987be1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6a6da80531cfbb45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6c280475c487a449
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6ca710681f0db6fb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6d1f6902c744386f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6fb1dd7faeee0f98
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6fd8649e4e08a08
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/72ebc4636e7ac7be
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/73f0aac8fb55b6ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/77a336face0ec4f1
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7d930974c8e253d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7dbd668b9f492d3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7f4b4829ba20a516
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8117798897b9ed6d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8260832a118d10dc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8305556502d2ea45
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8475b82408d2ee54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/855a7b58ef0544ec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/86c3273e51072d3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/877853d4dc81f361
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/88dbf7a942a9da64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/89d595309b4b7b68
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8e8cefaabb8a4bb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/95ca40290aa6c953
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/95fd5ea7b9e5dfb3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/9db82954adbe850b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/9f504d0ffc92dcfb
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a1142c359e181a9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a1a41619be06ccb4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a24137a45a8743b1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a2f215bbc4cc0d40
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a4787245a21ffe63
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a4875c83cb7271f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a54359630edfacd6
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a68ba8f5f87dc608
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a924d16624f6adf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/abf21f3f84ad1df4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ae41f6f26033f4bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/af9b4ba2d0453cda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b1152a95cbf2d4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b16ef8eaf80b86ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b2fe59c75a454b7e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b782bb5920ed7631
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ba44a3c3b3ac38d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c07ac676dcd21496
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c1d760c0cfb41438
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c276d1d063a64727
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c647c1c6c09ad625
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c85f693897ea918c
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c8c3aed8bad1198b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c91989c6d2d7a8a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cd137e47823314dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cdc22caf17ec54d3
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ce702570cde74416
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cef88f7047b583d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cf82bbe7c7c1adf9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d1d46e5a18de7d3a
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d446985a27be26f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d4fc514a2f18d78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/dc6404189af0c24c
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/dc6c6508ff33b09a
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/de63806b2b73c0f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/def645b0042e6c87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e0fec072417f247c
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e3414fe664479570
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e63ec54ef0702676
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e762d40f1905c5a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e8da77cd8ff6c797
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e928828d422ec175
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ea455768c753b5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/eb90c6985bd660dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ec8abef61a13d59f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/efab3295776f4a9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f0214717fe422ca0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f2daa6f6d8a29e8d
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f378cd188d3b89c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f44daa5adc10db55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f45513d4e62e04c1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f502d4daab623491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f7c55dccb7414089
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f9d56765099deab8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fc57508d0201a413
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fd85a9498d4d4764
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fdad3b8deea4269
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ffaf3bb26cb3b723
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/bundle.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/client.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/duration.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/nextup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/search.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/token.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/unwatched.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_bundle.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_client.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_duration.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_nextup.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_search.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_token.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_unwatched.py
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.client.yaml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
+-rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.client.yaml
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.client.yaml
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_single_term.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.4.0/LICENSE
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jellyash-0.4.0/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jellyash-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 jellyash-0.4.0/PKG-INFO
```

### Comparing `jellyash-0.3.4/LICENSE` & `jellyash-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.4/PKG-INFO` & `jellyash-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: jellyash
-Version: 0.3.4
+Version: 0.4.0
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
         
-        
-Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Python: >=3.7
+Requires-Dist: jellyfin-apiclient-python
+Requires-Dist: typing-extensions; python_version < '3.11'
+Description-Content-Type: text/markdown
 
 # Jellyash
 
 Jelly **A**eroplane **S**hark **H**elper
 
 Wrapper around jellyfin-apiclient-python to provide convenience functions:
```

### Comparing `jellyash-0.3.4/README.md` & `jellyash-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.4/jellyash/bundle.py` & `jellyash-0.4.0/jellyash/bundle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from typing import Dict, Iterator, Union
 
-if sys.version_info >= (3, 11):
+if sys.version_info >= (3, 11):  # pragma: no cover
     from typing import Self
 else:
     from typing_extensions import Self
 
 from jellyfin_apiclient_python.api import API
 
 
@@ -35,14 +35,17 @@
 
     def __iter__(self) -> Iterator[Item]:
         yield from [Item(i) for i in self.value["Items"]]
 
     def __getitem__(self, key) -> Item:
         return Item(self.value["Items"][key])
 
+    def _raw_value(self):
+        return self.value
+
     def __len__(self) -> int:
         return self.value["TotalRecordCount"] + self.value["StartIndex"]
 
 
 class WrappedAPI(API):
     def _get(self, handler, params=None):
         return ApiResponse(super()._get(handler, params=params))
```

### Comparing `jellyash-0.3.4/jellyash/client.py` & `jellyash-0.4.0/jellyash/client.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.4/jellyash/duration.py` & `jellyash-0.4.0/jellyash/duration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import argparse
 from decimal import Decimal
 
 from .client import authed_client
-from .series import search_single_show
+from .search import search_single_show
 
 
-def average_duration() -> None:
-    parser = argparse.ArgumentParser()
-    parser.add_argument("show", nargs="+")
-    args = parser.parse_args()
-    client = authed_client()
+def calculate_duration(client, show: str) -> str:
     try:
-        show = search_single_show(client, " ".join(args.show))
+        show = search_single_show(client, show)
     except ValueError as e:
-        print(str(e))
-        return
+        return str(e)
     count = 0
     duration = 0
     for season in client.jellyfin.get_seasons(show.Id):
         count += season.ChildCount
         episodes = client.jellyfin.get_season(show.Id, season.Id)
         duration += sum([e.RunTimeTicks for e in episodes])
     average = (duration / count) / int(Decimal("6E+008"))
-    print(f"Average duration over {count} episodes: {average:.1f} minutes")
+    return f"Average duration over {count} episodes: {average:.1f} minutes"
+
+
+def average_duration() -> None:
+    parser = argparse.ArgumentParser()
+    parser.add_argument("show", nargs="+")
+    args = parser.parse_args()
+    client = authed_client()
+    print(calculate_duration(client, " ".join(args.show)))
```

### Comparing `jellyash-0.3.4/jellyash/nextup.py` & `jellyash-0.4.0/jellyash/nextup.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.4/jellyash/token.py` & `jellyash-0.4.0/jellyash/token.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.3.4/jellyash/unwatched.py` & `jellyash-0.4.0/jellyash/unwatched.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from operator import attrgetter
 
 from .client import authed_client
-from .series import search_single_show
+from .search import search_single_show
 
 
 def unwatched() -> None:
     client = authed_client()
     parser = argparse.ArgumentParser()
     parser.add_argument("show", nargs="*")
     args = parser.parse_args()
@@ -22,20 +22,23 @@
     )
     total = 0
     for series in sorted(r, key=attrgetter("Name")):
         if (count := series.UserData.UnplayedItemCount) > 0:
             ending = "s" if count != 1 else ""
             print(f"{series.Name}: {count} unwatched episode{ending}")
             total += count
-    print(f"Total: {total} unwatched episodes")
+    ending = "s" if total != 1 else ""
+    print(f"Total: {total} unwatched episode{ending}")
 
 
 def specific_unwatched(client, term: str) -> None:
     try:
         show = search_single_show(client, term)
     except ValueError as e:
         print(str(e))
         return
     unwatched = show.UserData.UnplayedItemCount
     total = sum(s.ChildCount for s in client.jellyfin.get_seasons(show.Id))
-    print(f"{show.Name}: {total - unwatched} watched episodes")
-    print(f"{show.Name}: {unwatched} unwatched episodes")
+    ending = "s" if total - unwatched != 1 else ""
+    print(f"{show.Name}: {total - unwatched} watched episode{ending}")
+    ending = "s" if unwatched != 1 else ""
+    print(f"{show.Name}: {unwatched} unwatched episode{ending}")
```

### Comparing `jellyash-0.3.4/tests/test_client.py` & `jellyash-0.4.0/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import json
 import pathlib
 import platform
 import tempfile
 import unittest
 from unittest.mock import patch
 
+from jellyfin_apiclient_python.client import JellyfinClient
 import pytest
 
 from jellyash import __version__
 from jellyash.client import (
-    auth_with_password, auth_with_token, create_client
+    authed_client, auth_with_password, auth_with_token, create_client,
+    determine_app_name
     )
+from .conftest import ClientTest
 
 
 class TestClient(unittest.TestCase):
     def setUp(self):
         self.client = create_client("test")
 
     def test_create_client_with_app_name(self):
@@ -62,7 +65,32 @@
                     auth_with_token(None)
 
     def test_auth_with_nonexistant_file(self):
         non_exist = pathlib.Path("/does/not/exist")
         with patch("jellyash.client.CREDENTIALS_FILE", non_exist):
             with self.assertRaises(ValueError):
                 auth_with_token(None)
+
+
+class TestAuthedClient(ClientTest):
+    @pytest.mark.vcr
+    def test_authed_client(self):
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            credentials = self.test_client.auth.credentials.get_credentials()
+            with open(tmpfile.name, 'w') as f:
+                json.dump(credentials["Servers"][0], f)
+            ptf = pathlib.Path(tmpfile.name)
+            with patch("jellyash.client.CREDENTIALS_FILE", ptf):
+                client = authed_client()
+                self.assertTrue(isinstance(client, JellyfinClient))
+
+    def test_authed_client_non_existant_file(self):
+        non_exist = pathlib.Path("/does/not/exist")
+        with patch("jellyash.client.CREDENTIALS_FILE", non_exist):
+            with patch("sys.exit", return_value=None) as mock_exit:
+                authed_client()
+                mock_exit.assert_called_once()
+
+
+class TestDetermineAppName(unittest.TestCase):
+    def test_determine_app_name(self):
+        self.assertEqual(determine_app_name(), "jellyfin___init__")
```

