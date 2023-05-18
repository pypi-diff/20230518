# Comparing `tmp/tuack-0.1.5.1.tar.gz` & `tmp/tuack-0.1.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuack-0.1.5.1.tar", last modified: Tue May 16 13:21:22 2023, max compression
+gzip compressed data, was "tuack-0.1.5.1.1.tar", last modified: Thu May 18 04:25:50 2023, max compression
```

## Comparing `tuack-0.1.5.1.tar` & `tuack-0.1.5.1.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.256579 tuack-0.1.5.1/
--rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1/LICENSE
--rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0      520 2023-05-16 13:21:22.256579 tuack-0.1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-01-09 01:26:59.000000 tuack-0.1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 13:21:22.257586 tuack-0.1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1928 2023-05-16 13:21:02.000000 tuack-0.1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.176746 tuack-0.1.5.1/tuack/
--rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/__init__.py
--rw-rw-rw-   0        0        0    34497 2023-05-16 13:16:53.000000 tuack-0.1.5.1/tuack/base.py
--rw-rw-rw-   0        0        0    13348 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/doc.py
--rw-rw-rw-   0        0        0    27596 2023-05-13 08:34:57.000000 tuack-0.1.5.1/tuack/dump.py
--rw-rw-rw-   0        0        0    14486 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/gen.py
--rw-rw-rw-   0        0        0     2334 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/install.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.210316 tuack-0.1.5.1/tuack/lex/
--rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1/tuack/lex/compile.log
--rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/compile.pyinc
--rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-linux
--rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-mac
--rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/format-win.exe
--rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1/tuack/lex/hehe.log
--rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/lex.l
--rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/lex.yy.c
--rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1/tuack/lex/lex.yy.o
--rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/main.h
--rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.c
--rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.h
--rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1/tuack/lex/yacc.tab.o
--rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/lex/yacc.y
--rw-rw-rw-   0        0        0    12225 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/load.py
--rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/num2chinese.py
--rw-rw-rw-   0        0        0    12659 2023-05-16 13:14:46.000000 tuack-0.1.5.1/tuack/packer.py
--rw-rw-rw-   0        0        0    24468 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/ren.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.220544 tuack-0.1.5.1/tuack/sample/
--rw-rw-rw-   0        0        0     7909 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/arbiter_e.noi_linux1.sample
--rw-rw-rw-   0        0        0    23576 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/arbiter_e.sample
--rw-rw-rw-   0        0        0     5586 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/chk.cpp
--rw-rw-rw-   0        0        0      195 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/contest.gitignore
--rw-rw-rw-   0        0        0      266 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/contest.json
--rw-rw-rw-   0        0        0      186 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/day.gitignore
--rw-rw-rw-   0        0        0      207 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/day.json
--rw-rw-rw-   0        0        0      351 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.gitignore
--rw-rw-rw-   0        0        0      435 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/empty.json
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.234636 tuack-0.1.5.1/tuack/sample/precautions/
--rw-rw-rw-   0        0        0       60 2022-08-12 11:20:32.000000 tuack-0.1.5.1/tuack/sample/precautions/zh-cn.md
--rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/sample/problem.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/problem.gitignore
--rw-rw-rw-   0        0        0      466 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample/problem.json
--rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/sample/uoj.json
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.152628 tuack-0.1.5.1/tuack/sample-empty/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.222273 tuack-0.1.5.1/tuack/sample-empty/statement/
--rw-rw-rw-   0        0        0      411 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-empty/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.160667 tuack-0.1.5.1/tuack/sample-problem/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.223275 tuack-0.1.5.1/tuack/sample-problem/data/
--rw-rw-rw-   0        0        0       44 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/data/1.ans
--rw-rw-rw-   0        0        0       43 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/data/1.in
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.224930 tuack-0.1.5.1/tuack/sample-problem/down/
--rw-rw-rw-   0        0        0       79 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/down/1.ans
--rw-rw-rw-   0        0        0       77 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/down/1.in
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.225943 tuack-0.1.5.1/tuack/sample-problem/pre/
--rw-rw-rw-   0        0        0       80 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/pre/1.ans
--rw-rw-rw-   0        0        0       78 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/pre/1.in
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.226955 tuack-0.1.5.1/tuack/sample-problem/resources/
--rw-rw-rw-   0        0        0  3293583 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/resources/sample.png
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.229927 tuack-0.1.5.1/tuack/sample-problem/solution/
--rw-rw-rw-   0        0        0     1968 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/solution/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.229927 tuack-0.1.5.1/tuack/sample-problem/statement/
--rw-rw-rw-   0        0        0     6819 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/sample-problem/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.233563 tuack-0.1.5.1/tuack/sample-problem/tables/
--rw-rw-rw-   0        0        0     1062 2023-03-28 10:24:11.000000 tuack-0.1.5.1/tuack/sample-problem/tables/data.pyinc
--rw-rw-rw-   0        0        0     1227 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/tables/json_data.json
--rw-rw-rw-   0        0        0      205 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/sample-problem/tables/table.json
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.253127 tuack-0.1.5.1/tuack/templates/
--rw-rw-rw-   0        0        0      911 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/ccc.tex.jinja
--rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/templates/ccpc.png
--rw-rw-rw-   0        0        0     1240 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/ccpc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.162049 tuack-0.1.5.1/tuack/templates/en/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.254124 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/font.html.jinja
--rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/font.tex.jinja
--rw-rw-rw-   0        0        0      670 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/hand.tex.jinja
--rw-rw-rw-   0        0        0      144 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/image.html.jinja
--rw-rw-rw-   0        0        0      530 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/image.tex.jinja
--rw-rw-rw-   0        0        0     5116 2023-05-13 04:24:01.000000 tuack-0.1.5.1/tuack/templates/problem_base.md.jinja
--rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/table.html.jinja
--rw-rw-rw-   0        0        0      402 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/table.md.jinja
--rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1/tuack/templates/table.tex.jinja
--rw-rw-rw-   0        0        0     2125 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/template_base.tex.jinja
--rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1/tuack/templates/template_base.tex.jinja.tex
--rw-rw-rw-   0        0        0     4756 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tuack.cls
--rw-rw-rw-   0        0        0     8743 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tuoi.tex.jinja
--rw-rw-rw-   0        0        0     1443 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/tupc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.162312 tuack-0.1.5.1/tuack/templates/zh-cn/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.255580 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3139 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3543 2023-01-09 01:26:59.000000 tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0    17692 2023-01-09 01:27:42.000000 tuack-0.1.5.1/tuack/test.py
--rw-rw-rw-   0        0        0     3777 2023-02-22 09:36:20.000000 tuack-0.1.5.1/tuack/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:21:22.192980 tuack-0.1.5.1/tuack.egg-info/
--rw-rw-rw-   0        0        0      520 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-05-16 13:21:22.000000 tuack-0.1.5.1/tuack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 13:21:21.000000 tuack-0.1.5.1/tuack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:50.007295 tuack-0.1.5.1.1/
+-rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      522 2023-05-18 04:25:50.006298 tuack-0.1.5.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1717 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-18 04:25:50.007295 tuack-0.1.5.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1930 2023-05-18 04:25:25.000000 tuack-0.1.5.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.639522 tuack-0.1.5.1.1/tuack/
+-rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/__init__.py
+-rw-rw-rw-   0        0        0    34993 2023-05-18 04:24:36.000000 tuack-0.1.5.1.1/tuack/base.py
+-rw-rw-rw-   0        0        0    13348 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/doc.py
+-rw-rw-rw-   0        0        0    27596 2023-05-16 13:23:14.000000 tuack-0.1.5.1.1/tuack/dump.py
+-rw-rw-rw-   0        0        0    14486 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/gen.py
+-rw-rw-rw-   0        0        0     2334 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/install.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.770818 tuack-0.1.5.1.1/tuack/lex/
+-rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1.1/tuack/lex/compile.log
+-rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/compile.pyinc
+-rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-linux
+-rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-mac
+-rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-win.exe
+-rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1.1/tuack/lex/hehe.log
+-rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/lex.l
+-rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/lex.yy.c
+-rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1.1/tuack/lex/lex.yy.o
+-rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/main.h
+-rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.c
+-rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.h
+-rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.o
+-rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/yacc.y
+-rw-rw-rw-   0        0        0    12225 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/load.py
+-rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/num2chinese.py
+-rw-rw-rw-   0        0        0    13010 2023-05-16 13:23:14.000000 tuack-0.1.5.1.1/tuack/packer.py
+-rw-rw-rw-   0        0        0    24468 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/ren.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.836571 tuack-0.1.5.1.1/tuack/sample/
+-rw-rw-rw-   0        0        0     7909 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/arbiter_e.noi_linux1.sample
+-rw-rw-rw-   0        0        0    23576 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/arbiter_e.sample
+-rw-rw-rw-   0        0        0     5586 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/chk.cpp
+-rw-rw-rw-   0        0        0      195 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/contest.gitignore
+-rw-rw-rw-   0        0        0      266 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/contest.json
+-rw-rw-rw-   0        0        0      186 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/day.gitignore
+-rw-rw-rw-   0        0        0      207 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/day.json
+-rw-rw-rw-   0        0        0      351 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.gitignore
+-rw-rw-rw-   0        0        0      435 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.json
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.891887 tuack-0.1.5.1.1/tuack/sample/precautions/
+-rw-rw-rw-   0        0        0       60 2022-08-12 11:20:32.000000 tuack-0.1.5.1.1/tuack/sample/precautions/zh-cn.md
+-rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/sample/problem.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/problem.gitignore
+-rw-rw-rw-   0        0        0      466 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/problem.json
+-rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/sample/uoj.json
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/sample-empty/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.836571 tuack-0.1.5.1.1/tuack/sample-empty/statement/
+-rw-rw-rw-   0        0        0      411 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-empty/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/sample-problem/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.846552 tuack-0.1.5.1.1/tuack/sample-problem/data/
+-rw-rw-rw-   0        0        0       44 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/data/1.ans
+-rw-rw-rw-   0        0        0       43 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/data/1.in
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.856917 tuack-0.1.5.1.1/tuack/sample-problem/down/
+-rw-rw-rw-   0        0        0       79 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/down/1.ans
+-rw-rw-rw-   0        0        0       77 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/down/1.in
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.866375 tuack-0.1.5.1.1/tuack/sample-problem/pre/
+-rw-rw-rw-   0        0        0       80 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/pre/1.ans
+-rw-rw-rw-   0        0        0       78 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/pre/1.in
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.873787 tuack-0.1.5.1.1/tuack/sample-problem/resources/
+-rw-rw-rw-   0        0        0  3293583 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/resources/sample.png
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.876780 tuack-0.1.5.1.1/tuack/sample-problem/solution/
+-rw-rw-rw-   0        0        0     1968 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/solution/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.877777 tuack-0.1.5.1.1/tuack/sample-problem/statement/
+-rw-rw-rw-   0        0        0     6819 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/sample-problem/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.890900 tuack-0.1.5.1.1/tuack/sample-problem/tables/
+-rw-rw-rw-   0        0        0     1062 2023-03-28 10:24:11.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/data.pyinc
+-rw-rw-rw-   0        0        0     1227 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/json_data.json
+-rw-rw-rw-   0        0        0      205 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/table.json
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.982673 tuack-0.1.5.1.1/tuack/templates/
+-rw-rw-rw-   0        0        0      911 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/ccc.tex.jinja
+-rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/templates/ccpc.png
+-rw-rw-rw-   0        0        0     1240 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/ccpc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/templates/en/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.993341 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/font.html.jinja
+-rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/font.tex.jinja
+-rw-rw-rw-   0        0        0      670 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/hand.tex.jinja
+-rw-rw-rw-   0        0        0      144 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/image.html.jinja
+-rw-rw-rw-   0        0        0      530 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/image.tex.jinja
+-rw-rw-rw-   0        0        0     5116 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/templates/problem_base.md.jinja
+-rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/table.html.jinja
+-rw-rw-rw-   0        0        0      402 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/table.md.jinja
+-rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/templates/table.tex.jinja
+-rw-rw-rw-   0        0        0     2125 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja
+-rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja.tex
+-rw-rw-rw-   0        0        0     4756 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tuack.cls
+-rw-rw-rw-   0        0        0     8743 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tuoi.tex.jinja
+-rw-rw-rw-   0        0        0     1443 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tupc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/templates/zh-cn/
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:50.004314 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3139 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3543 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0    17497 2023-05-18 04:24:36.000000 tuack-0.1.5.1.1/tuack/test.py
+-rw-rw-rw-   0        0        0     3777 2023-02-22 09:36:20.000000 tuack-0.1.5.1.1/tuack/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.645500 tuack-0.1.5.1.1/tuack.egg-info/
+-rw-rw-rw-   0        0        0      522 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/top_level.txt
```

### Comparing `tuack-0.1.5.1/LICENSE` & `tuack-0.1.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/PKG-INFO` & `tuack-0.1.5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1
+Version: 0.1.5.1.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1/README.md` & `tuack-0.1.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/setup.py` & `tuack-0.1.5.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	'pyyaml >= 5.1',
 	'rarfile >= 3.0',
 	'requests_toolbelt >= 0.9.1'
 ]
 
 setup(
 	name = 'tuack',
-	version = '0.1.5.1',
+	version = '0.1.5.1.1',
 	packages = find_packages(),
 	author = 'Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan',
 	author_email = 'chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn',
 	url = '',
 	license = 'https://git.thusaac.com/publish/tuack/blob/master/LICENSE',
 	description = 'Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.',
 	cmdclass={
```

### Comparing `tuack-0.1.5.1/tuack/base.py` & `tuack-0.1.5.1.1/tuack/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from multiprocessing import Process, Queue
 from functools import wraps
 from threading import Timer
 import platform
 import logging
 import traceback
 import yaml
-from inspect import isfunction
+from inspect import isfunction, getsource
 
 python_version = (sys.version_info.major, sys.version_info.minor, sys.version_info.micro)
 if python_version[0] == 2:
 	reload(sys)
 	sys.setdefaultencoding('utf-8')
 
 class Memory(str):
@@ -1008,7 +1008,29 @@
 def run_exc(func):
 	try:
 		return (True, func())
 	except Exception as e:
 		log.error(e)
 		log.info(traceback.format_exc())
 		return (False, None)
+
+def rmtree(path):
+	if os.path.exists(path):
+		if system == 'Windows':
+			os.system(f'rmdir /s /q "{path}"')
+		else:
+			shutil.rmtree(path)
+
+def repeat(func):
+	las = None
+	for i in range(10):
+		try:
+			func()
+		except Exception as e:
+			las = e
+			time.sleep(1e-2)
+			log.warning(f'执行该函数第{i + 1}次：' + func.__qualname__)
+		else:
+			return
+	log.error('重复执行该函数多次失败：' + func.__qualname__)
+	log.info(getsource(func))
+	raise las
```

### Comparing `tuack-0.1.5.1/tuack/doc.py` & `tuack-0.1.5.1.1/tuack/doc.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/dump.py` & `tuack-0.1.5.1.1/tuack/dump.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/gen.py` & `tuack-0.1.5.1.1/tuack/gen.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/install.py` & `tuack-0.1.5.1.1/tuack/install.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/compile.pyinc` & `tuack-0.1.5.1.1/tuack/lex/compile.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/format-linux` & `tuack-0.1.5.1.1/tuack/lex/format-linux`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/format-mac` & `tuack-0.1.5.1.1/tuack/lex/format-mac`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/format-win.exe` & `tuack-0.1.5.1.1/tuack/lex/format-win.exe`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/lex.l` & `tuack-0.1.5.1.1/tuack/lex/lex.l`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/lex.yy.c` & `tuack-0.1.5.1.1/tuack/lex/lex.yy.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/lex.yy.o` & `tuack-0.1.5.1.1/tuack/lex/lex.yy.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/yacc.tab.c` & `tuack-0.1.5.1.1/tuack/lex/yacc.tab.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/yacc.tab.h` & `tuack-0.1.5.1.1/tuack/lex/yacc.tab.h`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/lex/yacc.tab.o` & `tuack-0.1.5.1.1/tuack/lex/yacc.tab.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/load.py` & `tuack-0.1.5.1.1/tuack/load.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/num2chinese.py` & `tuack-0.1.5.1.1/tuack/num2chinese.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/packer.py` & `tuack-0.1.5.1.1/tuack/packer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,351 +1,351 @@
-# -*- coding: utf-8 -*-
-
-from __future__ import print_function
-import os
-import re
-import sys
-import json
-import datetime
-import shutil
-import subprocess
-import time
-import signal
-import zipfile
-from multiprocessing import Process, Queue
-from functools import wraps
-from threading import Timer
-import platform
-from .base import *
-from . import base
-import math
-
-doc_format = re.compile(r'^(.*)\.(doc|docs|ppt|pptx|pdf|tex|md|html|htm|zip|dir)$')
-empty_cpp = 'int main(){}'
-
-def find_doc(path, name):
-	for f in os.listdir(path):
-		m = doc_format.match(f)
-		if m and m.group(1) == name:
-			return name, '.' + m.group(2)
-	return None
-
-def test_copy_problem_files(prob):
-	data_path = os.path.join(prob.path, 'data')
-	try:
-		copy(data_path, 'chk', base.pjoin(output_folder, prob.route))
-		prob.chk = True
-	except base.NoInstalledException as e:
-		raise(e)
-	except Exception as e:
-		prob.chk = False
-	
-def copy_one_day_files(probs, day_name):
-	remkdir(os.path.join(output_folder, day_name, 'data'))
-	print('copy data files')
-	for prob in probs:
-		if base.rjoin(day_name, prob['name']) not in base.prob_set:
-			continue
-		# TODO: if test cases is a list of scores instead of an integer
-		data_path = os.path.join(day_name, prob['name'], 'data')
-		for i in range(1, prob['test cases'] + 1):
-			for suf in ['.in', '.ans']:
-				copy(data_path, prob['name'] + str(i) + suf, os.path.join(output_folder, day_name, 'data'))
-		copy(data_path, 'chk', os.path.join(output_folder, day_name, 'data', prob['name'] + '_e'))
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, os.path.join(output_folder, day_name, 'data'))
-	print('dos2unix data files')
-	if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, 'data', '*')) != 0:
-		warning('dos2unix failed.')
-	print('copy down files')
-	remkdir(os.path.join(output_folder, day_name, 'down'))
-	for prob in probs:
-		if base.rjoin(day_name, prob['name']) not in base.prob_set:
-			continue
-		# TODO: if test cases is a list of scores instead of an integer
-		data_path = os.path.join(day_name, prob['name'], 'down')
-		target_path = os.path.join(output_folder, day_name, 'down', prob['name'])
-		if not os.path.exists(target_path):
-			os.makedirs(target_path)
-		#print(prob)
-		case_no = (prob['test cases'] if prob['type'] == 'output' else prob['sample count'])
-		suffices = (['.in'] if prob['type'] == 'output' else ['.in', '.ans'])
-		for i in range(1, case_no + 1):
-			for suf in suffices:
-				copy(data_path, prob['name'] + str(i) + suf, target_path)
-		copy(data_path, 'checker', target_path)
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, target_path)
-	print('dos2unix down files')
-	for prob in probs:
-		if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, 'down', prob['name'], '*')) != 0:
-			warning('dos2unix failed.')
-			break
-	remkdir(os.path.join(output_folder, day_name, 'discussion'))
-	for prob in probs:
-		res = find_doc(os.path.join(day_name, prob['name']), 'discussion')
-		if res:
-			copy(os.path.join(day_name, prob['name']), res[0] + res[1], os.path.join(output_folder, day_name, 'discussion', prob['name'] + res[1]))
-		else:
-			warning('Can\'t find discussion ppt for problem `%s`.' % prob['name'])
-	if os.path.exists('log'):
-		os.remove('log')
-		
-def pc2_copy_one_day_files(probs, day_name):
-	remkdir(os.path.join('pc2', day_name))
-	remkdir(os.path.join('pc2', day_name, 'data'))
-	print('copy data files')
-	for prob in probs:
-		if base.rjoin(day_name, prob['name']) not in base.prob_set:
-			continue
-		name = prob['name'].capitalize()
-		# TODO: if test cases is a list of scores instead of an integer
-		remkdir(os.path.join('pc2', day_name, 'data', name))
-		data_path = os.path.join(day_name, name, 'data')
-		target_path = os.path.join('pc2', day_name, 'data', name)
-		for i in range(1, prob['test cases'] + 1):
-			for suf in ['.in', '.ans']:
-				copy(data_path, prob['name'] + str(i) + suf, target_path)
-		copy(data_path, 'chk', target_path)
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, target_path)
-		if os.system('dos2unix %s 2> log' % os.path.join(target_path, '*')) != 0:
-			warning('dos2unix failed.')
-	print('copy down files')
-	remkdir(os.path.join('pc2', day_name, 'down'))
-	for prob in probs:
-		if base.rjoin(day_name, prob['name']) not in base.prob_set:
-			continue
-		name = prob['name'].capitalize()
-		# TODO: if test cases is a list of scores instead of an integer
-		data_path = os.path.join(day_name, prob['name'], 'down')
-		target_path = os.path.join('pc2', day_name, 'down', name)
-		remkdir(target_path)
-		case_no = (prob['test cases'] if prob['type'] == 'output' else prob['sample count'])
-		suffices = (['.in'] if prob['type'] == 'output' else ['.in', '.ans'])
-		for i in range(1, case_no + 1):
-			for suf in suffices:
-				copy(data_path, prob['name'] + str(i) + suf, target_path)
-		copy(data_path, 'checker', target_path)
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, target_path)
-	print('dos2unix down files')
-	for prob in probs:
-		if os.system('dos2unix %s 2> log' % os.path.join('pc2', day_name, 'down', prob['name'], '*')) != 0:
-			warning('dos2unix failed.')
-			break
-	remkdir(os.path.join('pc2', day_name, 'discussion'))
-	for prob in probs:
-		res = find_doc(os.path.join(day_name, prob['name']), 'discussion')
-		if res:
-			copy(os.path.join(day_name, prob['name']), res[0] + res[1], os.path.join('pc2', day_name, 'discussion', prob['name'] + res[1]))
-		else:
-			warning('Can\'t find discussion ppt for problem `%s`.' % prob['name'])
-	if os.path.exists('log'):
-		os.remove('log')
-		
-def prob2uoj_conf(prob):
-	s = ''
-	s += 'use_builtin_judger on\n'
-	if 'uoj checker' not in prob:
-		s += 'use_builtin_checker wcmp\n'
-	elif prob['uoj checker'] != False:
-		s += 'use_builtin_checker %s\n' % prob['uoj checker']
-	if prob['type'] == 'output':
-		s += 'submit_answer on\n'
-	s += 'n_tests %d\n' % prob['test cases']
-	s += 'n_ex_tests %d\n' % prob['sample count']
-	s += 'n_sample_tests %d\n' % prob['sample count']
-	s += 'input_pre %s\n' % prob['name']
-	s += 'input_suf in\n'
-	s += 'output_pre %s\n' % prob['name']
-	s += 'output_suf ans\n'
-	if 'time limit' in prob:
-		s += 'time_limit %d\n' % math.ceil(prob['time limit'])
-	if 'memory limit' in prob:
-		s += 'memory_limit %d\n' % (base.memory2bytes(prob['memory limit']) // 1024 // 1024)
-	if 'output limit' in prob:
-		s += 'output_limit %d\n' % (base.memory2bytes(prob['output limit']) // 1024 // 1024)
-	else:
-		s += 'output_limit 64\n'
-	return s
-
-def uoj_copy_one_day_files(probs, day_name):
-	print('copy data files')
-	for prob in probs:
-		if base.rjoin(day_name, prob['name']) not in base.prob_set:
-			continue
-		# TODO: if test cases is a list of scores instead of an integer
-		data_path = os.path.join(day_name, prob['name'], 'data')
-		target_path = os.path.join(output_folder, day_name, prob['name'], '1')
-		#remkdir(os.path.join(output_folder, day_name, prob['name']))
-		remkdir(target_path)
-		for i in range(1, prob['test cases'] + 1):
-			for suf in ['.in', '.ans']:
-				copy(data_path, prob['name'] + str(i) + suf, target_path)
-		if not copy(os.path.join(data_path, 'chk'), 'chk.cpp', target_path) and 'uoj_builtin_checker' not in prob:
-			prob['uoj_builtin_checker'] = 'wcmp'
-		if not copy(os.path.join(data_path, 'val'), 'val.cpp', target_path):
-			pass
-			#with open(os.path.join(target_path, 'val.cpp'), 'w') as f:
-			#	f.write(empty_cpp)
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				require_path = os.path.join(target_path, 'require')
-				if not os.path.exists(require_path):
-					os.makedirs(require_path)
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, require_path)
-		download_path = os.path.join(target_path, 'download')
-		remkdir(download_path)
-		case_no = (0 if prob['type'] == 'output' else prob['sample count'])
-		suffices = ['.in', '.ans']
-		data_path = os.path.join(day_name, prob['name'], 'down')
-		for i in range(1, case_no + 1):
-			for suf in suffices:
-				#copy(data_path, prob['name'] + str(i) + suf, download_path)
-				copy(data_path, prob['name'] + str(i) + suf, os.path.join(target_path, 'ex_' + prob['name'] + str(i) + suf))
-		copy(data_path, 'checker', download_path)
-		for name in os.listdir(data_path):
-			if os.path.join(data_path, name) not in base.copied_data:
-				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
-				copy(data_path, name, download_path)
-		with open(os.path.join(target_path, 'problem.conf'), 'w') as f:
-			f.write(prob2uoj_conf(prob))
-		#with open(os.path.join(target_path, 'std.cpp'), 'w') as f:
-		#	f.write(empty_cpp)
-		if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, prob['name'], '1', '*')) != 0:
-			warning('dos2unix failed.')
-	if os.path.exists('log'):
-		os.remove('log')
-
-def copy_files(suffix = ''):
-	for day in base.days():
-		base.mkdir(os.path.join(output_folder, day.route))
-	for prob in base.probs():
-		eval(suffix + 'copy_problem_files')(prob)
-
-def zip_tree(z, path):
-	for name in os.listdir(path):
-		full_path = os.path.join(path, name)
-		if os.path.isdir(full_path):
-			zip_tree(z, full_path)
-		else:
-			z.write(full_path)
-
-def make_zip():
-	for day_name, day_data in base.probs.items():
-		if day_name not in base.day_set:
-			continue
-		with zipfile.ZipFile(os.path.join(output_folder, day_name + '.zip'), 'w') as z:
-			zip_tree(z, os.path.join(output_folder, day_name))
-
-def noi():
-	global output_folder
-	base.no_compiling = False
-	output_folder = 'noi'
-	remkdir('noi')
-	copy_files()
-
-def test():
-	global output_folder
-	base.no_compiling = False
-	output_folder = 'bin'
-	if base.conf.folder != 'problem':
-		remkdir('bin')
-		for day in base.days():
-			remkdir(base.pjoin('bin', day.route))
-	copy_files('test_')
-	
-def pc2():
-	global output_folder
-	base.no_compiling = True
-	remkdir('pc2')
-	copy_files('pc2_')
-
-def release():
-	global output_folder
-	infom('make release files.')
-	remkdir('release')
-	base.no_compiling = True
-	output_folder = 'release'
-	copy_files()
-	make_zip()
-
-def svn_init():
-	for day_name, probs in base.probs.items():
-		if day_name not in base.day_set:
-			continue
-		for prob in probs:
-			if base.rjoin(day_name, prob['name']) not in base.prob_set:
-				continue
-			if not os.path.exists(os.path.join('uoj', day_name, prob['name'], '.svn')):
-				os.system(
-					'svn checkout --username %s --password %s %s %s' % (
-						uoj_config['user'],
-						uoj_config['svn pwd'],
-						'svn://%s/problem/%d' % (uoj_config['host'], prob['uoj id']),
-						os.path.join(os.path.join('uoj', day_name, prob['name']))
-					)
-				)
-			else:
-				os.system('svn delete %s' % os.path.join(os.path.join('uoj', day_name, prob['name'], '1')))
-	
-def svn_upload():
-	for day_name, probs in base.probs.items():
-		if day_name not in base.day_set:
-			continue
-		for prob in probs:
-			if base.rjoin(day_name, prob['name']) not in base.prob_set:
-				continue
-			os.system('svn add %s' % os.path.join(os.path.join('uoj', day_name, prob['name'], '1')))
-			os.system('svn commit %s -m "%s"' % (
-				os.path.join(os.path.join('uoj', day_name, prob['name'], '1')),
-				'Auto generated by oi_tools'
-			))
-
-def uoj():
-	global output_folder, uoj_config
-	base.no_compiling = False
-	output_folder = 'uoj'
-	if not os.path.exists('uoj'):
-		os.makedirs('uoj')
-	if not os.path.exists('uoj.json'):
-		flag = False
-		warning('uoj.json not found. Cannot upload to uoj')
-	else:
-		flag = True
-	if flag:
-		uoj_config = json.loads(open('uoj.json').read())
-		svn_init()
-	copy_files('uoj_')
-	if flag:
-		svn_upload()
-
-work_list = {
-	'noi' : noi,
-	'test' : test,
-	'uoj' : uoj,
-	'pc2' : pc2,
-	'release' : release
-}
-
-if __name__ == '__main__':
-	if base.init():
-		infom('Packing starts at %s.\n' % str(datetime.datetime.now()))
-		for base.work in base.works:
-			work_list[base.work]()
-	else:
-		print('Use arguments other than options to run what to output.')
-		print('Enabled output types:')
-		print('\ttest: Generate output for test. Must run this output before tester.py.')
-		print('\trelease: Generate what is suitable to publish.')
-		print('\tnoi: Generate output in noi style.')
-		print('\tuoj: Generate output in uoj style.')
+# -*- coding: utf-8 -*-
+
+from __future__ import print_function
+import os
+import re
+import sys
+import json
+import datetime
+import shutil
+import subprocess
+import time
+import signal
+import zipfile
+from multiprocessing import Process, Queue
+from functools import wraps
+from threading import Timer
+import platform
+from .base import *
+from . import base
+import math
+
+doc_format = re.compile(r'^(.*)\.(doc|docs|ppt|pptx|pdf|tex|md|html|htm|zip|dir)$')
+empty_cpp = 'int main(){}'
+
+def find_doc(path, name):
+	for f in os.listdir(path):
+		m = doc_format.match(f)
+		if m and m.group(1) == name:
+			return name, '.' + m.group(2)
+	return None
+
+def test_copy_problem_files(prob):
+	data_path = os.path.join(prob.path, 'data')
+	try:
+		copy(data_path, 'chk', base.pjoin(output_folder, prob.route))
+		prob.chk = True
+	except base.NoInstalledException as e:
+		raise(e)
+	except Exception as e:
+		prob.chk = False
+	
+def copy_one_day_files(probs, day_name):
+	remkdir(os.path.join(output_folder, day_name, 'data'))
+	print('copy data files')
+	for prob in probs:
+		if base.rjoin(day_name, prob['name']) not in base.prob_set:
+			continue
+		# TODO: if test cases is a list of scores instead of an integer
+		data_path = os.path.join(day_name, prob['name'], 'data')
+		for i in range(1, prob['test cases'] + 1):
+			for suf in ['.in', '.ans']:
+				copy(data_path, prob['name'] + str(i) + suf, os.path.join(output_folder, day_name, 'data'))
+		copy(data_path, 'chk', os.path.join(output_folder, day_name, 'data', prob['name'] + '_e'))
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, os.path.join(output_folder, day_name, 'data'))
+	print('dos2unix data files')
+	if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, 'data', '*')) != 0:
+		warning('dos2unix failed.')
+	print('copy down files')
+	remkdir(os.path.join(output_folder, day_name, 'down'))
+	for prob in probs:
+		if base.rjoin(day_name, prob['name']) not in base.prob_set:
+			continue
+		# TODO: if test cases is a list of scores instead of an integer
+		data_path = os.path.join(day_name, prob['name'], 'down')
+		target_path = os.path.join(output_folder, day_name, 'down', prob['name'])
+		if not os.path.exists(target_path):
+			os.makedirs(target_path)
+		#print(prob)
+		case_no = (prob['test cases'] if prob['type'] == 'output' else prob['sample count'])
+		suffices = (['.in'] if prob['type'] == 'output' else ['.in', '.ans'])
+		for i in range(1, case_no + 1):
+			for suf in suffices:
+				copy(data_path, prob['name'] + str(i) + suf, target_path)
+		copy(data_path, 'checker', target_path)
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, target_path)
+	print('dos2unix down files')
+	for prob in probs:
+		if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, 'down', prob['name'], '*')) != 0:
+			warning('dos2unix failed.')
+			break
+	remkdir(os.path.join(output_folder, day_name, 'discussion'))
+	for prob in probs:
+		res = find_doc(os.path.join(day_name, prob['name']), 'discussion')
+		if res:
+			copy(os.path.join(day_name, prob['name']), res[0] + res[1], os.path.join(output_folder, day_name, 'discussion', prob['name'] + res[1]))
+		else:
+			warning('Can\'t find discussion ppt for problem `%s`.' % prob['name'])
+	if os.path.exists('log'):
+		os.remove('log')
+		
+def pc2_copy_one_day_files(probs, day_name):
+	remkdir(os.path.join('pc2', day_name))
+	remkdir(os.path.join('pc2', day_name, 'data'))
+	print('copy data files')
+	for prob in probs:
+		if base.rjoin(day_name, prob['name']) not in base.prob_set:
+			continue
+		name = prob['name'].capitalize()
+		# TODO: if test cases is a list of scores instead of an integer
+		remkdir(os.path.join('pc2', day_name, 'data', name))
+		data_path = os.path.join(day_name, name, 'data')
+		target_path = os.path.join('pc2', day_name, 'data', name)
+		for i in range(1, prob['test cases'] + 1):
+			for suf in ['.in', '.ans']:
+				copy(data_path, prob['name'] + str(i) + suf, target_path)
+		copy(data_path, 'chk', target_path)
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, target_path)
+		if os.system('dos2unix %s 2> log' % os.path.join(target_path, '*')) != 0:
+			warning('dos2unix failed.')
+	print('copy down files')
+	remkdir(os.path.join('pc2', day_name, 'down'))
+	for prob in probs:
+		if base.rjoin(day_name, prob['name']) not in base.prob_set:
+			continue
+		name = prob['name'].capitalize()
+		# TODO: if test cases is a list of scores instead of an integer
+		data_path = os.path.join(day_name, prob['name'], 'down')
+		target_path = os.path.join('pc2', day_name, 'down', name)
+		remkdir(target_path)
+		case_no = (prob['test cases'] if prob['type'] == 'output' else prob['sample count'])
+		suffices = (['.in'] if prob['type'] == 'output' else ['.in', '.ans'])
+		for i in range(1, case_no + 1):
+			for suf in suffices:
+				copy(data_path, prob['name'] + str(i) + suf, target_path)
+		copy(data_path, 'checker', target_path)
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, target_path)
+	print('dos2unix down files')
+	for prob in probs:
+		if os.system('dos2unix %s 2> log' % os.path.join('pc2', day_name, 'down', prob['name'], '*')) != 0:
+			warning('dos2unix failed.')
+			break
+	remkdir(os.path.join('pc2', day_name, 'discussion'))
+	for prob in probs:
+		res = find_doc(os.path.join(day_name, prob['name']), 'discussion')
+		if res:
+			copy(os.path.join(day_name, prob['name']), res[0] + res[1], os.path.join('pc2', day_name, 'discussion', prob['name'] + res[1]))
+		else:
+			warning('Can\'t find discussion ppt for problem `%s`.' % prob['name'])
+	if os.path.exists('log'):
+		os.remove('log')
+		
+def prob2uoj_conf(prob):
+	s = ''
+	s += 'use_builtin_judger on\n'
+	if 'uoj checker' not in prob:
+		s += 'use_builtin_checker wcmp\n'
+	elif prob['uoj checker'] != False:
+		s += 'use_builtin_checker %s\n' % prob['uoj checker']
+	if prob['type'] == 'output':
+		s += 'submit_answer on\n'
+	s += 'n_tests %d\n' % prob['test cases']
+	s += 'n_ex_tests %d\n' % prob['sample count']
+	s += 'n_sample_tests %d\n' % prob['sample count']
+	s += 'input_pre %s\n' % prob['name']
+	s += 'input_suf in\n'
+	s += 'output_pre %s\n' % prob['name']
+	s += 'output_suf ans\n'
+	if 'time limit' in prob:
+		s += 'time_limit %d\n' % math.ceil(prob['time limit'])
+	if 'memory limit' in prob:
+		s += 'memory_limit %d\n' % (base.memory2bytes(prob['memory limit']) // 1024 // 1024)
+	if 'output limit' in prob:
+		s += 'output_limit %d\n' % (base.memory2bytes(prob['output limit']) // 1024 // 1024)
+	else:
+		s += 'output_limit 64\n'
+	return s
+
+def uoj_copy_one_day_files(probs, day_name):
+	print('copy data files')
+	for prob in probs:
+		if base.rjoin(day_name, prob['name']) not in base.prob_set:
+			continue
+		# TODO: if test cases is a list of scores instead of an integer
+		data_path = os.path.join(day_name, prob['name'], 'data')
+		target_path = os.path.join(output_folder, day_name, prob['name'], '1')
+		#remkdir(os.path.join(output_folder, day_name, prob['name']))
+		remkdir(target_path)
+		for i in range(1, prob['test cases'] + 1):
+			for suf in ['.in', '.ans']:
+				copy(data_path, prob['name'] + str(i) + suf, target_path)
+		if not copy(os.path.join(data_path, 'chk'), 'chk.cpp', target_path) and 'uoj_builtin_checker' not in prob:
+			prob['uoj_builtin_checker'] = 'wcmp'
+		if not copy(os.path.join(data_path, 'val'), 'val.cpp', target_path):
+			pass
+			#with open(os.path.join(target_path, 'val.cpp'), 'w') as f:
+			#	f.write(empty_cpp)
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				require_path = os.path.join(target_path, 'require')
+				if not os.path.exists(require_path):
+					os.makedirs(require_path)
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, require_path)
+		download_path = os.path.join(target_path, 'download')
+		remkdir(download_path)
+		case_no = (0 if prob['type'] == 'output' else prob['sample count'])
+		suffices = ['.in', '.ans']
+		data_path = os.path.join(day_name, prob['name'], 'down')
+		for i in range(1, case_no + 1):
+			for suf in suffices:
+				#copy(data_path, prob['name'] + str(i) + suf, download_path)
+				copy(data_path, prob['name'] + str(i) + suf, os.path.join(target_path, 'ex_' + prob['name'] + str(i) + suf))
+		copy(data_path, 'checker', download_path)
+		for name in os.listdir(data_path):
+			if os.path.join(data_path, name) not in base.copied_data:
+				warning('Unusual file \'%s\' found.' % os.path.join(data_path, name))
+				copy(data_path, name, download_path)
+		with open(os.path.join(target_path, 'problem.conf'), 'w') as f:
+			f.write(prob2uoj_conf(prob))
+		#with open(os.path.join(target_path, 'std.cpp'), 'w') as f:
+		#	f.write(empty_cpp)
+		if os.system('dos2unix %s 2> log' % os.path.join(output_folder, day_name, prob['name'], '1', '*')) != 0:
+			warning('dos2unix failed.')
+	if os.path.exists('log'):
+		os.remove('log')
+
+def copy_files(suffix = ''):
+	for day in base.days():
+		base.mkdir(os.path.join(output_folder, day.route))
+	for prob in base.probs():
+		eval(suffix + 'copy_problem_files')(prob)
+
+def zip_tree(z, path):
+	for name in os.listdir(path):
+		full_path = os.path.join(path, name)
+		if os.path.isdir(full_path):
+			zip_tree(z, full_path)
+		else:
+			z.write(full_path)
+
+def make_zip():
+	for day_name, day_data in base.probs.items():
+		if day_name not in base.day_set:
+			continue
+		with zipfile.ZipFile(os.path.join(output_folder, day_name + '.zip'), 'w') as z:
+			zip_tree(z, os.path.join(output_folder, day_name))
+
+def noi():
+	global output_folder
+	base.no_compiling = False
+	output_folder = 'noi'
+	remkdir('noi')
+	copy_files()
+
+def test():
+	global output_folder
+	base.no_compiling = False
+	output_folder = 'bin'
+	if base.conf.folder != 'problem':
+		remkdir('bin')
+		for day in base.days():
+			remkdir(base.pjoin('bin', day.route))
+	copy_files('test_')
+	
+def pc2():
+	global output_folder
+	base.no_compiling = True
+	remkdir('pc2')
+	copy_files('pc2_')
+
+def release():
+	global output_folder
+	infom('make release files.')
+	remkdir('release')
+	base.no_compiling = True
+	output_folder = 'release'
+	copy_files()
+	make_zip()
+
+def svn_init():
+	for day_name, probs in base.probs.items():
+		if day_name not in base.day_set:
+			continue
+		for prob in probs:
+			if base.rjoin(day_name, prob['name']) not in base.prob_set:
+				continue
+			if not os.path.exists(os.path.join('uoj', day_name, prob['name'], '.svn')):
+				os.system(
+					'svn checkout --username %s --password %s %s %s' % (
+						uoj_config['user'],
+						uoj_config['svn pwd'],
+						'svn://%s/problem/%d' % (uoj_config['host'], prob['uoj id']),
+						os.path.join(os.path.join('uoj', day_name, prob['name']))
+					)
+				)
+			else:
+				os.system('svn delete %s' % os.path.join(os.path.join('uoj', day_name, prob['name'], '1')))
+	
+def svn_upload():
+	for day_name, probs in base.probs.items():
+		if day_name not in base.day_set:
+			continue
+		for prob in probs:
+			if base.rjoin(day_name, prob['name']) not in base.prob_set:
+				continue
+			os.system('svn add %s' % os.path.join(os.path.join('uoj', day_name, prob['name'], '1')))
+			os.system('svn commit %s -m "%s"' % (
+				os.path.join(os.path.join('uoj', day_name, prob['name'], '1')),
+				'Auto generated by oi_tools'
+			))
+
+def uoj():
+	global output_folder, uoj_config
+	base.no_compiling = False
+	output_folder = 'uoj'
+	if not os.path.exists('uoj'):
+		os.makedirs('uoj')
+	if not os.path.exists('uoj.json'):
+		flag = False
+		warning('uoj.json not found. Cannot upload to uoj')
+	else:
+		flag = True
+	if flag:
+		uoj_config = json.loads(open('uoj.json').read())
+		svn_init()
+	copy_files('uoj_')
+	if flag:
+		svn_upload()
+
+work_list = {
+	'noi' : noi,
+	'test' : test,
+	'uoj' : uoj,
+	'pc2' : pc2,
+	'release' : release
+}
+
+if __name__ == '__main__':
+	if base.init():
+		infom('Packing starts at %s.\n' % str(datetime.datetime.now()))
+		for base.work in base.works:
+			work_list[base.work]()
+	else:
+		print('Use arguments other than options to run what to output.')
+		print('Enabled output types:')
+		print('\ttest: Generate output for test. Must run this output before tester.py.')
+		print('\trelease: Generate what is suitable to publish.')
+		print('\tnoi: Generate output in noi style.')
+		print('\tuoj: Generate output in uoj style.')
```

### Comparing `tuack-0.1.5.1/tuack/ren.py` & `tuack-0.1.5.1.1/tuack/ren.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample/arbiter_e.noi_linux1.sample` & `tuack-0.1.5.1.1/tuack/sample/arbiter_e.noi_linux1.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample/arbiter_e.sample` & `tuack-0.1.5.1.1/tuack/sample/arbiter_e.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample/chk.cpp` & `tuack-0.1.5.1.1/tuack/sample/chk.cpp`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample-problem/resources/sample.png` & `tuack-0.1.5.1.1/tuack/sample-problem/resources/sample.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample-problem/solution/zh-cn.md` & `tuack-0.1.5.1.1/tuack/sample-problem/solution/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample-problem/statement/zh-cn.md` & `tuack-0.1.5.1.1/tuack/sample-problem/statement/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample-problem/tables/data.pyinc` & `tuack-0.1.5.1.1/tuack/sample-problem/tables/data.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/sample-problem/tables/json_data.json` & `tuack-0.1.5.1.1/tuack/sample-problem/tables/json_data.json`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/ccc.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/ccc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/ccpc.png` & `tuack-0.1.5.1.1/tuack/templates/ccpc.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/ccpc.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/ccpc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/en/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/hand.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/hand.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/image.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/image.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/problem_base.md.jinja` & `tuack-0.1.5.1.1/tuack/templates/problem_base.md.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/table.html.jinja` & `tuack-0.1.5.1.1/tuack/templates/table.html.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/table.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/table.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/template_base.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/tuack.cls` & `tuack-0.1.5.1.1/tuack/templates/tuack.cls`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/tuoi.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/tuoi.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/tupc.tex.jinja` & `tuack-0.1.5.1.1/tuack/templates/tupc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack/test.py` & `tuack-0.1.5.1.1/tuack/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,27 +376,17 @@
 				if not expe or len(expe) == 0:
 					log.warning(u'程序`%s/%s`没有设置期望得分。' % (user, algo))
 					log.info(u'如果该程序是标程、部分分程序或骗分程序等，需要设置它的`expected`字段。')
 					log.info(u'有多种设置的格式，例如：`== 60`表示该程序应该得到60分。')
 					log.info(u'如果该程序是其他功能程序，例如数据生成器，请将该程序从配置文件中移除。')
 				if (not prob.all and match != 1 and not base.any_prefix(rjoin(prob.route, user, algo))):
 					continue
-				while os.path.exists('tmp'):
-					try:
-						shutil.rmtree('tmp')
-					except:
-						time.sleep(1e-2)
+				base.repeat(lambda : base.rmtree('tmp'))
 				if prob['type'] == 'program':
-					while True:
-						try:
-							os.makedirs('tmp')
-						except:
-							time.sleep(1e-2)
-						else:
-							break
+					base.repeat(lambda : os.makedirs('tmp'))
 					try:
 						shutil.copy(path, pjoin('tmp', path.split('/')[-1]))
 					except Exception as e:
 						log.error(u'程序`%s`没有找到。' % path)
 						log.info(e)
 						log.info(u'如果该程序是测试程序，请确保该程序存在；如果不是，请将其从`conf.*`中移除。')
 						continue
@@ -411,19 +401,15 @@
 						else:
 							break
 					else:
 						log.error(u'跳过该输出文件包。')
 						log.info(u'如果该文件包是测试输出，请确保该文件包存在；如果不是，请将其从`conf.*`中移除。')
 				log.info(u'测试程序 %s:%s:%s' % (prob['name'], user, algo))
 				scores, times, reports = test(prob, path.split('/')[-1].split('.')[0])
-				while os.path.exists('tmp'):
-					try:
-						shutil.rmtree('tmp')
-					except:
-						pass
+				base.repeat(lambda : base.rmtree('tmp'))
 				tc = len(prob.test_cases)
 				score_map = {}
 				for i in range(tc):
 					score_map[prob.test_cases[i]] = i
 				if prob.packed:
 					packed = packed_score(scores[:tc], times[:tc], reports[:tc], score_map, prob)
 					tot = sum(packed[0][:-1])
```

### Comparing `tuack-0.1.5.1/tuack/tools.py` & `tuack-0.1.5.1.1/tuack/tools.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1/tuack.egg-info/PKG-INFO` & `tuack-0.1.5.1.1/tuack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1
+Version: 0.1.5.1.1
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1/tuack.egg-info/SOURCES.txt` & `tuack-0.1.5.1.1/tuack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

