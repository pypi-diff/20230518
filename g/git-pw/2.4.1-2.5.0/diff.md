# Comparing `tmp/git-pw-2.4.1.tar.gz` & `tmp/git-pw-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-pw-2.4.1.tar", last modified: Mon May  8 11:21:11 2023, max compression
+gzip compressed data, was "git-pw-2.5.0.tar", last modified: Thu May 18 14:07:42 2023, max compression
```

## Comparing `git-pw-2.4.1.tar` & `git-pw-2.5.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 11:21:01.000000 git-pw-2.4.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.320402 git-pw-2.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.320402 git-pw-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-08 11:21:01.000000 git-pw-2.4.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 11:21:01.000000 git-pw-2.4.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 11:21:01.000000 git-pw-2.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-08 11:21:11.000000 git-pw-2.4.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-08 11:21:11.000000 git-pw-2.4.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-08 11:21:01.000000 git-pw-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 11:21:11.332403 git-pw-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-08 11:21:01.000000 git-pw-2.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 11:21:01.000000 git-pw-2.4.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/git_pw/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-08 11:21:01.000000 git-pw-2.4.1/git_pw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.324402 git-pw-2.4.1/git_pw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 11:21:11.000000 git-pw-2.4.1/git_pw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.328403 git-pw-2.4.1/man/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-add.1
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-create.1
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-delete.1
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-download.1
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-remove.1
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-show.1
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle-update.1
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-bundle.1
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-download.1
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-show.1
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch-update.1
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-patch.1
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-apply.1
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-download.1
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-list.1
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series-show.1
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw-series.1
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-08 11:21:01.000000 git-pw-2.4.1/man/git-pw.1
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:01.000000 git-pw-2.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.328403 git-pw-2.4.1/releasenotes/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/add-yaml-format-support-5cd6b9028e6d2d8e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/api-v1-1-5c804713ef435739.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/bundle-crud-47aadae6eb7a20ad.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-pypy-support-f670deb05ef527fe.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-python-35-36-support-add-python-310-7d364b9ba71bf5ba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/drop-python34-support-5e01360fff605972.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/enforce-filtering-by-project-59ed29c4b7edc0a5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/filter-item-list-by-user-id-4f4e7d6dc402093b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/filter-multiple-matches-197ff839f6b578da.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/handle-error-codes-d72c575fb2d9b452.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/initial-release-0aad09064615d023.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-24-60a9fa796f666f35.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-29-884269fdf35f64b2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-40-add82959d7442cfa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-43-c2c166e1fa23fe76.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-44-66b78577e9534f16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-46-50933643cd5c8db0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-47-a9ac87642050d289.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-48-694495f722119fed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-49-865c4f1657b97fce.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/issue-55-bfcf05e02ad305b1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/passthrough-git-am-arguments-23cd0b292304d648.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/patch-apply-applyPatchDeps-option-9a8fed887af313d5.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/patch-states-b88240569f8474f1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/python-2-deprecation-c87e311384eab29b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/python-311-support-de330cb1ff9da396.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/random-fixes-3da473a63c253f2d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/remove-python-3-2-3-3-support-8987031bed2c0333.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/require-server-version-93ac0818c293b85e.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/save-patches-before-applying-c5e786156d47d752.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/update-multiple-patches-ed515cd53964c203.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/use-bundle-names-b1b3ee5c2858c96b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/use-git-pager-settings-ec6555d8311a8bec.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-08 11:21:01.000000 git-pw-2.4.1/releasenotes/notes/warn-on-multiple-filters-a4e01fdb5cf6e459.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:21:01.000000 git-pw-2.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-08 11:21:01.000000 git-pw-2.4.1/rpm/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 11:21:01.000000 git-pw-2.4.1/rpm/git-pw.spec
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-08 11:21:11.332403 git-pw-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 11:21:01.000000 git-pw-2.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:21:01.000000 git-pw-2.4.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:11.332403 git-pw-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19499 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-08 11:21:01.000000 git-pw-2.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 11:21:01.000000 git-pw-2.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.449804 git-pw-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 14:07:32.000000 git-pw-2.5.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.437804 git-pw-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.441804 git-pw-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-18 14:07:32.000000 git-pw-2.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 14:07:32.000000 git-pw-2.5.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 14:07:32.000000 git-pw-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 14:07:42.000000 git-pw-2.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-18 14:07:42.000000 git-pw-2.5.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-18 14:07:32.000000 git-pw-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-18 14:07:42.453804 git-pw-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-18 14:07:32.000000 git-pw-2.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.441804 git-pw-2.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 14:07:32.000000 git-pw-2.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.441804 git-pw-2.5.0/git_pw/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-18 14:07:32.000000 git-pw-2.5.0/git_pw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.445804 git-pw-2.5.0/git_pw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 14:07:42.000000 git-pw-2.5.0/git_pw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.445804 git-pw-2.5.0/man/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-add.1
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-create.1
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-delete.1
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-remove.1
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle-update.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-bundle.1
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch-update.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-patch.1
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-series-apply.1
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-series-download.1
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-series-list.1
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-series-show.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw-series.1
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-18 14:07:32.000000 git-pw-2.5.0/man/git-pw.1
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 14:07:32.000000 git-pw-2.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.445804 git-pw-2.5.0/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.449804 git-pw-2.5.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/add-before-since-options-c67799ef2ad89c0c.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/add-yaml-format-support-5cd6b9028e6d2d8e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/api-v1-1-5c804713ef435739.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/bundle-crud-47aadae6eb7a20ad.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/drop-pypy-support-f670deb05ef527fe.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/drop-python-35-36-support-add-python-310-7d364b9ba71bf5ba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/drop-python34-support-5e01360fff605972.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/enforce-filtering-by-project-59ed29c4b7edc0a5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/filter-item-list-by-user-id-4f4e7d6dc402093b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/filter-multiple-matches-197ff839f6b578da.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/handle-error-codes-d72c575fb2d9b452.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/initial-release-0aad09064615d023.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-24-60a9fa796f666f35.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-29-884269fdf35f64b2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-40-add82959d7442cfa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-43-c2c166e1fa23fe76.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-44-66b78577e9534f16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-46-50933643cd5c8db0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-47-a9ac87642050d289.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-48-694495f722119fed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-49-865c4f1657b97fce.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/issue-55-bfcf05e02ad305b1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/passthrough-git-am-arguments-23cd0b292304d648.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/patch-apply-applyPatchDeps-option-9a8fed887af313d5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/patch-states-b88240569f8474f1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/python-2-deprecation-c87e311384eab29b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/python-311-support-de330cb1ff9da396.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/random-fixes-3da473a63c253f2d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/remove-python-3-2-3-3-support-8987031bed2c0333.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/require-server-version-93ac0818c293b85e.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/save-patches-before-applying-c5e786156d47d752.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/update-multiple-patches-ed515cd53964c203.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/use-bundle-names-b1b3ee5c2858c96b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/use-git-pager-settings-ec6555d8311a8bec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 14:07:32.000000 git-pw-2.5.0/releasenotes/notes/warn-on-multiple-filters-a4e01fdb5cf6e459.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 14:07:32.000000 git-pw-2.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.449804 git-pw-2.5.0/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-18 14:07:32.000000 git-pw-2.5.0/rpm/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-18 14:07:32.000000 git-pw-2.5.0/rpm/git-pw.spec
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-18 14:07:42.453804 git-pw-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 14:07:32.000000 git-pw-2.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 14:07:32.000000 git-pw-2.5.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:42.449804 git-pw-2.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19499 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/test_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-18 14:07:32.000000 git-pw-2.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-18 14:07:32.000000 git-pw-2.5.0/tox.ini
```

### Comparing `git-pw-2.4.1/.github/workflows/ci.yaml` & `git-pw-2.5.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/.pre-commit-config.yaml` & `git-pw-2.5.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ---
 default_language_version:
   # force all unspecified python hooks to run python3
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
```

### Comparing `git-pw-2.4.1/ChangeLog` & `git-pw-2.5.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+2.5.0
+-----
+
+* Release 2.5.0
+* Add release note for --since, --before opts
+* patch, series: Add support for '--since' and '--before'
+* Bump pre-commit
+
 2.4.1
 -----
 
 * Release 2.4.1
 * CI: Address deprecation warning
 * CI: Use modern contexts
 * CI: Reintroduce publishing to Test PyPI
```

### Comparing `git-pw-2.4.1/LICENSE` & `git-pw-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/PKG-INFO` & `git-pw-2.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pw
-Version: 2.4.1
+Version: 2.5.0
 Summary: Git-Patchwork integration tool
 Home-page: https://github.com/getpatchwork/git-pw
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/getpatchwork/git-pw/issues
 Project-URL: Source Code, https://github.com/getpatchwork/git-pw
```

### Comparing `git-pw-2.4.1/README.rst` & `git-pw-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/docs/conf.py` & `git-pw-2.5.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # git-pw documentation build configuration file
 
 import git_pw
 
 try:
     import sphinx_rtd_theme  # noqa
+
     has_rtd_theme = True
 except ImportError:
     has_rtd_theme = False
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
```

### Comparing `git-pw-2.4.1/git_pw/api.py` & `git-pw-2.5.0/git_pw/api.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/git_pw/bundle.py` & `git-pw-2.5.0/git_pw/bundle.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/git_pw/config.py` & `git-pw-2.5.0/git_pw/config.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/git_pw/patch.py` & `git-pw-2.5.0/git_pw/patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,24 +325,27 @@
 )
 @click.option(
     '--archived',
     default=False,
     is_flag=True,
     help='Include patches that are archived.',
 )
+@utils.date_options()
 @utils.pagination_options(sort_fields=_sort_fields, default_sort='-date')
 @utils.format_options(headers=_list_headers)
 @click.argument('name', required=False)
 @api.validate_multiple_filter_support
 def list_cmd(
     states,
     submitters,
     delegates,
     hashes,
     archived,
+    since,
+    before,
     limit,
     page,
     sort,
     fmt,
     headers,
     name,
 ):
@@ -399,14 +402,20 @@
             ('archived', 'true' if archived else 'false'),
             ('page', page),
             ('per_page', limit),
             ('order', sort),
         ]
     )
 
+    if since:
+        params.append(('since', since.isoformat()))
+
+    if before:
+        params.append(('before', before.isoformat()))
+
     patches = api.index('patches', params)
 
     # Format and print output
 
     output = []
 
     for patch in patches:
```

### Comparing `git-pw-2.4.1/git_pw/series.py` & `git-pw-2.5.0/git_pw/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,19 +157,20 @@
     metavar='SUBMITTER',
     multiple=True,
     help=(
         'Show only series by these submitters. Should be an '
         'email, name or ID.'
     ),
 )
+@utils.date_options()
 @utils.pagination_options(sort_fields=_sort_fields, default_sort='-date')
 @utils.format_options(headers=_list_headers)
 @click.argument('name', required=False)
 @api.validate_multiple_filter_support
-def list_cmd(submitters, limit, page, sort, fmt, headers, name):
+def list_cmd(submitters, limit, page, sort, fmt, headers, name, since, before):
     """List series.
 
     List series on the Patchwork instance.
     """
     LOG.debug(
         'List series: submitters=%s, limit=%r, page=%r, sort=%r',
         ','.join(submitters),
@@ -197,14 +198,20 @@
             ('q', name),
             ('page', page),
             ('per_page', limit),
             ('order', sort),
         ]
     )
 
+    if since:
+        params.append(('since', since.isoformat()))
+
+    if before:
+        params.append(('before', before.isoformat()))
+
     series = api.index('series', params)
 
     # Format and print output
 
     output = []
 
     for series_ in series:
```

### Comparing `git-pw-2.4.1/git_pw/shell.py` & `git-pw-2.5.0/git_pw/shell.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/git_pw/utils.py` & `git-pw-2.5.0/git_pw/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -203,14 +203,36 @@
         )(f)
 
         return f
 
     return _pagination_options
 
 
+def date_options() -> ty.Callable:
+    """Shared date bounding options."""
+
+    def _date_options(f):
+        f = click.option(
+            '--since',
+            metavar='SINCE',
+            type=click.DateTime(),
+            help='Show only items since a given date in ISO 8601 format',
+        )(f)
+        f = click.option(
+            '--before',
+            metavar='BEFORE',
+            type=click.DateTime(),
+            help='Show only items before a given date in ISO 8601 format',
+        )(f)
+
+        return f
+
+    return _date_options
+
+
 def format_options(
     original_function: ty.Optional[ty.Callable] = None,
     headers: ty.Optional[ty.Tuple[str, ...]] = None,
 ) -> ty.Callable:
     """Shared output format options."""
 
     def _format_options(f):
```

### Comparing `git-pw-2.4.1/git_pw.egg-info/PKG-INFO` & `git-pw-2.5.0/git_pw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-pw
-Version: 2.4.1
+Version: 2.5.0
 Summary: Git-Patchwork integration tool
 Home-page: https://github.com/getpatchwork/git-pw
 Author: Stephen Finucane
 Author-email: stephen@that.guru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/getpatchwork/git-pw/issues
 Project-URL: Source Code, https://github.com/getpatchwork/git-pw
```

### Comparing `git-pw-2.4.1/git_pw.egg-info/SOURCES.txt` & `git-pw-2.5.0/git_pw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 man/git-pw-series-apply.1
 man/git-pw-series-download.1
 man/git-pw-series-list.1
 man/git-pw-series-show.1
 man/git-pw-series.1
 man/git-pw.1
 releasenotes/config.yaml
+releasenotes/notes/add-before-since-options-c67799ef2ad89c0c.yaml
 releasenotes/notes/add-yaml-format-support-5cd6b9028e6d2d8e.yaml
 releasenotes/notes/api-v1-1-5c804713ef435739.yaml
 releasenotes/notes/bundle-crud-47aadae6eb7a20ad.yaml
 releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml
 releasenotes/notes/drop-pypy-support-f670deb05ef527fe.yaml
 releasenotes/notes/drop-python-35-36-support-add-python-310-7d364b9ba71bf5ba.yaml
 releasenotes/notes/drop-python34-support-5e01360fff605972.yaml
```

### Comparing `git-pw-2.4.1/man/git-pw-bundle-create.1` & `git-pw-2.5.0/man/git-pw-bundle-create.1`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE CREATE" "1" "2023-05-08" "2.4.1" "git-pw bundle create Manual"
+.TH "GIT-PW BUNDLE CREATE" "1" "2023-05-18" "2.5.0" "git-pw bundle create Manual"
 .SH NAME
 git-pw\-bundle\-create \- Create a bundle.
 .SH SYNOPSIS
 .B git-pw bundle create
 [OPTIONS] NAME PATCH_IDS...
 .SH DESCRIPTION
 Create a bundle.
```

### Comparing `git-pw-2.4.1/man/git-pw-bundle-list.1` & `git-pw-2.5.0/man/git-pw-bundle-list.1`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE LIST" "1" "2023-05-08" "2.4.1" "git-pw bundle list Manual"
+.TH "GIT-PW BUNDLE LIST" "1" "2023-05-18" "2.5.0" "git-pw bundle list Manual"
 .SH NAME
 git-pw\-bundle\-list \- List bundles.
 .SH SYNOPSIS
 .B git-pw bundle list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List bundles.
```

### Comparing `git-pw-2.4.1/man/git-pw-bundle-remove.1` & `git-pw-2.5.0/man/git-pw-bundle-remove.1`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE REMOVE" "1" "2023-05-08" "2.4.1" "git-pw bundle remove Manual"
+.TH "GIT-PW BUNDLE REMOVE" "1" "2023-05-18" "2.5.0" "git-pw bundle remove Manual"
 .SH NAME
 git-pw\-bundle\-remove \- Remove one or more patches from a bundle.
 .SH SYNOPSIS
 .B git-pw bundle remove
 [OPTIONS] BUNDLE_ID PATCH_IDS...
 .SH DESCRIPTION
 Remove one or more patches from a bundle.
```

### Comparing `git-pw-2.4.1/man/git-pw-bundle-update.1` & `git-pw-2.5.0/man/git-pw-bundle-update.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE UPDATE" "1" "2023-05-08" "2.4.1" "git-pw bundle update Manual"
+.TH "GIT-PW BUNDLE UPDATE" "1" "2023-05-18" "2.5.0" "git-pw bundle update Manual"
 .SH NAME
 git-pw\-bundle\-update \- Update a bundle.
 .SH SYNOPSIS
 .B git-pw bundle update
 [OPTIONS] BUNDLE_ID
 .SH DESCRIPTION
 Update a bundle.
```

### Comparing `git-pw-2.4.1/man/git-pw-bundle.1` & `git-pw-2.5.0/man/git-pw-bundle.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW BUNDLE" "1" "2023-05-08" "2.4.1" "git-pw bundle Manual"
+.TH "GIT-PW BUNDLE" "1" "2023-05-18" "2.5.0" "git-pw bundle Manual"
 .SH NAME
 git-pw\-bundle \- Interact with bundles.
 .SH SYNOPSIS
 .B git-pw bundle
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with bundles.
```

### Comparing `git-pw-2.4.1/man/git-pw-patch-apply.1` & `git-pw-2.5.0/man/git-pw-patch-apply.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH APPLY" "1" "2023-05-08" "2.4.1" "git-pw patch apply Manual"
+.TH "GIT-PW PATCH APPLY" "1" "2023-05-18" "2.5.0" "git-pw patch apply Manual"
 .SH NAME
 git-pw\-patch\-apply \- Apply patch.
 .SH SYNOPSIS
 .B git-pw patch apply
 [OPTIONS] PATCH_ID [ARGS]...
 .SH DESCRIPTION
 Apply patch.
```

### Comparing `git-pw-2.4.1/man/git-pw-patch-download.1` & `git-pw-2.5.0/man/git-pw-patch-download.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH DOWNLOAD" "1" "2023-05-08" "2.4.1" "git-pw patch download Manual"
+.TH "GIT-PW PATCH DOWNLOAD" "1" "2023-05-18" "2.5.0" "git-pw patch download Manual"
 .SH NAME
 git-pw\-patch\-download \- Download patch in diff or mbox format.
 .SH SYNOPSIS
 .B git-pw patch download
 [OPTIONS] PATCH_ID [OUTPUT]
 .SH DESCRIPTION
 Download patch in diff or mbox format.
```

### Comparing `git-pw-2.4.1/man/git-pw-patch-list.1` & `git-pw-2.5.0/man/git-pw-patch-list.1`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH LIST" "1" "2023-05-08" "2.4.1" "git-pw patch list Manual"
+.TH "GIT-PW PATCH LIST" "1" "2023-05-18" "2.5.0" "git-pw patch list Manual"
 .SH NAME
 git-pw\-patch\-list \- List patches.
 .SH SYNOPSIS
 .B git-pw patch list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List patches.
@@ -22,14 +22,20 @@
 .TP
 \fB\-\-hash\fP HASH
 Show only patches with these hashes.
 .TP
 \fB\-\-archived\fP
 Include patches that are archived.
 .TP
+\fB\-\-before\fP BEFORE
+Show only items before a given date in ISO 8601 format
+.TP
+\fB\-\-since\fP SINCE
+Show only items since a given date in ISO 8601 format
+.TP
 \fB\-\-sort\fP FIELD
 Sort output on given field.
 .TP
 \fB\-\-page\fP PAGE
 Page to retrieve items from. This is influenced by the size of LIMIT.
 .TP
 \fB\-\-limit\fP LIMIT
```

### Comparing `git-pw-2.4.1/man/git-pw-patch-update.1` & `git-pw-2.5.0/man/git-pw-patch-update.1`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH UPDATE" "1" "2023-05-08" "2.4.1" "git-pw patch update Manual"
+.TH "GIT-PW PATCH UPDATE" "1" "2023-05-18" "2.5.0" "git-pw patch update Manual"
 .SH NAME
 git-pw\-patch\-update \- Update one or more patches.
 .SH SYNOPSIS
 .B git-pw patch update
 [OPTIONS] PATCH_IDS...
 .SH DESCRIPTION
 Update one or more patches.
```

### Comparing `git-pw-2.4.1/man/git-pw-patch.1` & `git-pw-2.5.0/man/git-pw-patch.1`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW PATCH" "1" "2023-05-08" "2.4.1" "git-pw patch Manual"
+.TH "GIT-PW PATCH" "1" "2023-05-18" "2.5.0" "git-pw patch Manual"
 .SH NAME
 git-pw\-patch \- Interact with patches.
 .SH SYNOPSIS
 .B git-pw patch
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with patches.
```

### Comparing `git-pw-2.4.1/man/git-pw-series-download.1` & `git-pw-2.5.0/man/git-pw-series-download.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES DOWNLOAD" "1" "2023-05-08" "2.4.1" "git-pw series download Manual"
+.TH "GIT-PW SERIES DOWNLOAD" "1" "2023-05-18" "2.5.0" "git-pw series download Manual"
 .SH NAME
 git-pw\-series\-download \- Download series in mbox format.
 .SH SYNOPSIS
 .B git-pw series download
 [OPTIONS] SERIES_ID [OUTPUT]
 .SH DESCRIPTION
 Download series in mbox format.
```

### Comparing `git-pw-2.4.1/man/git-pw-series-list.1` & `git-pw-2.5.0/man/git-pw-series-list.1`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES LIST" "1" "2023-05-08" "2.4.1" "git-pw series list Manual"
+.TH "GIT-PW SERIES LIST" "1" "2023-05-18" "2.5.0" "git-pw series list Manual"
 .SH NAME
 git-pw\-series\-list \- List series.
 .SH SYNOPSIS
 .B git-pw series list
 [OPTIONS] [NAME]
 .SH DESCRIPTION
 List series.
@@ -10,14 +10,20 @@
     List series on the Patchwork instance.
 
 .SH OPTIONS
 .TP
 \fB\-\-submitter\fP SUBMITTER
 Show only series by these submitters. Should be an email, name or ID.
 .TP
+\fB\-\-before\fP BEFORE
+Show only items before a given date in ISO 8601 format
+.TP
+\fB\-\-since\fP SINCE
+Show only items since a given date in ISO 8601 format
+.TP
 \fB\-\-sort\fP FIELD
 Sort output on given field.
 .TP
 \fB\-\-page\fP PAGE
 Page to retrieve items from. This is influenced by the size of LIMIT.
 .TP
 \fB\-\-limit\fP LIMIT
```

### Comparing `git-pw-2.4.1/man/git-pw-series.1` & `git-pw-2.5.0/man/git-pw-series.1`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW SERIES" "1" "2023-05-08" "2.4.1" "git-pw series Manual"
+.TH "GIT-PW SERIES" "1" "2023-05-18" "2.5.0" "git-pw series Manual"
 .SH NAME
 git-pw\-series \- Interact with series.
 .SH SYNOPSIS
 .B git-pw series
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 Interact with series.
```

### Comparing `git-pw-2.4.1/man/git-pw.1` & `git-pw-2.5.0/man/git-pw.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GIT-PW" "1" "2023-05-08" "2.4.1" "git-pw Manual"
+.TH "GIT-PW" "1" "2023-05-18" "2.5.0" "git-pw Manual"
 .SH NAME
 git-pw \- git-pw is a tool for integrating Git with...
 .SH SYNOPSIS
 .B git-pw
 [OPTIONS] COMMAND [ARGS]...
 .SH DESCRIPTION
 git-pw is a tool for integrating Git with Patchwork.
```

### Comparing `git-pw-2.4.1/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml` & `git-pw-2.5.0/releasenotes/notes/download-series-to-separate-patches-eae647315dd4d2e1.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml` & `git-pw-2.5.0/releasenotes/notes/save-patches-to-file-c667ab7dd0b73ead.yaml`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/rpm/README.rst` & `git-pw-2.5.0/rpm/README.rst`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/rpm/git-pw.spec` & `git-pw-2.5.0/rpm/git-pw.spec`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/setup.cfg` & `git-pw-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/tests/test_api.py` & `git-pw-2.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/tests/test_bundle.py` & `git-pw-2.5.0/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/tests/test_patch.py` & `git-pw-2.5.0/tests/test_patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -387,14 +387,18 @@
                 '--limit',
                 1,
                 '--page',
                 1,
                 '--sort',
                 '-name',
                 'test',
+                '--since',
+                '2022-01-01',
+                '--before',
+                '2022-12-31',
             ],
         )
 
         assert result.exit_code == 0, result
         calls = [
             mock.call('people', [('q', 'john@example.com')]),
             mock.call('users', [('q', 'doe@example.com')]),
@@ -408,14 +412,16 @@
                     ('delegate', '2'),
                     ('hash', 'foo'),
                     ('q', 'test'),
                     ('archived', 'true'),
                     ('page', 1),
                     ('per_page', 1),
                     ('order', '-name'),
+                    ('since', '2022-01-01T00:00:00'),
+                    ('before', '2022-12-31T00:00:00'),
                 ],
             ),
         ]
 
         mock_index.assert_has_calls(calls)
 
     @mock.patch('git_pw.api.LOG')
```

### Comparing `git-pw-2.4.1/tests/test_series.py` & `git-pw-2.5.0/tests/test_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,18 @@
                 '--limit',
                 1,
                 '--page',
                 1,
                 '--sort',
                 '-name',
                 'test',
+                '--since',
+                '2022-01-01',
+                '--before',
+                '2022-12-31',
             ],
         )
 
         assert result.exit_code == 0, result
         calls = [
             mock.call('people', [('q', 'john@example.com')]),
             mock.call(
@@ -237,14 +241,16 @@
                 [
                     ('submitter', 1),
                     ('submitter', '2'),
                     ('q', 'test'),
                     ('page', 1),
                     ('per_page', 1),
                     ('order', '-name'),
+                    ('since', '2022-01-01T00:00:00'),
+                    ('before', '2022-12-31T00:00:00'),
                 ],
             ),
         ]
 
         mock_index.assert_has_calls(calls)
 
     @mock.patch('git_pw.api.LOG')
```

### Comparing `git-pw-2.4.1/tests/test_utils.py` & `git-pw-2.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `git-pw-2.4.1/tox.ini` & `git-pw-2.5.0/tox.ini`

 * *Files identical despite different names*

