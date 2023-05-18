# Comparing `tmp/limnoria-2023.1.28.tar.gz` & `tmp/limnoria-2023.4.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limnoria-2023.1.28.tar", last modified: Sat Feb 11 09:15:17 2023, max compression
+gzip compressed data, was "limnoria-2023.4.28.tar", last modified: Thu May 18 13:06:35 2023, max compression
```

## Comparing `limnoria-2023.1.28.tar` & `limnoria-2023.4.28.tar`

### file list

```diff
@@ -1,757 +1,767 @@
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.752235 limnoria-2023.1.28/
--rw-r--r--   0 val       (1000) val       (1000)     1654 2023-02-11 09:14:15.000000 limnoria-2023.1.28/LICENSE.md
--rw-r--r--   0 val       (1000) val       (1000)      117 2023-02-11 09:14:15.000000 limnoria-2023.1.28/MANIFEST.in
--rw-r--r--   0 val       (1000) val       (1000)      983 2023-02-11 09:14:15.000000 limnoria-2023.1.28/Makefile
--rw-r--r--   0 val       (1000) val       (1000)     1764 2023-02-11 09:15:17.752235 limnoria-2023.1.28/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)     2292 2023-02-11 09:14:15.000000 limnoria-2023.1.28/README.md
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/limnoria.egg-info/
--rw-r--r--   0 val       (1000) val       (1000)     1764 2023-02-11 09:15:17.000000 limnoria-2023.1.28/limnoria.egg-info/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)    15946 2023-02-11 09:15:17.000000 limnoria-2023.1.28/limnoria.egg-info/SOURCES.txt
--rw-r--r--   0 val       (1000) val       (1000)        1 2023-02-11 09:15:17.000000 limnoria-2023.1.28/limnoria.egg-info/dependency_links.txt
--rw-r--r--   0 val       (1000) val       (1000)        8 2023-02-11 09:15:17.000000 limnoria-2023.1.28/limnoria.egg-info/top_level.txt
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/locales/
--rw-r--r--   0 val       (1000) val       (1000)        0 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    54113 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    76337 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    77441 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3749 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/fr.py
--rw-r--r--   0 val       (1000) val       (1000)    69991 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    42399 2023-02-11 09:14:15.000000 limnoria-2023.1.28/locales/messages.pot
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/man/
--rw-r--r--   0 val       (1000) val       (1000)     1183 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-adduser.1
--rw-r--r--   0 val       (1000) val       (1000)     1468 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-botchk.1
--rw-r--r--   0 val       (1000) val       (1000)     1111 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-plugin-create.1
--rw-r--r--   0 val       (1000) val       (1000)     1364 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-plugin-doc.1
--rw-r--r--   0 val       (1000) val       (1000)     1016 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-reset-password.1
--rw-r--r--   0 val       (1000) val       (1000)     1485 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-test.1
--rw-r--r--   0 val       (1000) val       (1000)     1177 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot-wizard.1
--rw-r--r--   0 val       (1000) val       (1000)     1958 2023-02-11 09:14:15.000000 limnoria-2023.1.28/man/supybot.1
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/plugins/
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/plugins/Admin/
--rw-r--r--   0 val       (1000) val       (1000)     2422 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2312 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.660234 limnoria-2023.1.28/plugins/Admin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8064 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8857 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7809 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8112 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15152 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5897 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Admin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Aka/
--rw-r--r--   0 val       (1000) val       (1000)     2788 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Aka/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Aka/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Aka/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11022 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Aka/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    39586 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Aka/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14785 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Aka/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Alias/
--rw-r--r--   0 val       (1000) val       (1000)     2655 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2539 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Alias/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4716 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5751 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5059 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5176 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     4919 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19130 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8039 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Alias/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Anonymous/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3516 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.664234 limnoria-2023.1.28/plugins/Anonymous/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6558 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7384 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5903 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6893 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     6535 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9054 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6882 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Anonymous/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/AutoMode/
--rw-r--r--   0 val       (1000) val       (1000)     2697 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4521 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/AutoMode/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4202 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5058 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4512 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4131 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8029 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/AutoMode/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/Autocomplete/
--rw-r--r--   0 val       (1000) val       (1000)     2946 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Autocomplete/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2808 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Autocomplete/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6158 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Autocomplete/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6635 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Autocomplete/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/BadWords/
--rw-r--r--   0 val       (1000) val       (1000)     2695 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6163 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/BadWords/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6862 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6112 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6277 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7475 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3943 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/BadWords/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/Channel/
--rw-r--r--   0 val       (1000) val       (1000)     2480 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3497 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.668234 limnoria-2023.1.28/plugins/Channel/locales/
--rw-r--r--   0 val       (1000) val       (1000)    32456 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    35277 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    32166 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    32899 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    33333 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    44412 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13344 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Channel/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/ChannelLogger/
--rw-r--r--   0 val       (1000) val       (1000)     2531 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5994 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/ChannelLogger/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5491 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5340 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5607 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5183 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    13745 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9242 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelLogger/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/ChannelStats/
--rw-r--r--   0 val       (1000) val       (1000)     2682 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3449 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/ChannelStats/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6426 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6640 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6242 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15391 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4870 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ChannelStats/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/Conditional/
--rw-r--r--   0 val       (1000) val       (1000)     2907 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2763 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/Conditional/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8160 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7180 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7493 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11342 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6497 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Conditional/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.672234 limnoria-2023.1.28/plugins/Config/
--rw-r--r--   0 val       (1000) val       (1000)     2325 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Config/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9209 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     9329 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     9265 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    21747 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    25531 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Config/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Ctcp/
--rw-r--r--   0 val       (1000) val       (1000)     2420 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3652 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Ctcp/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2084 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2196 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2072 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2073 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     1911 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7136 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1785 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Ctcp/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/DDG/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/DDG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3332 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/DDG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6037 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/DDG/parser.py
--rw-r--r--   0 val       (1000) val       (1000)     6988 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/DDG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2389 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/DDG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Debug/
--rw-r--r--   0 val       (1000) val       (1000)     2377 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Debug/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2399 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Debug/config.py
--rw-r--r--   0 val       (1000) val       (1000)     7272 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Debug/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2648 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Debug/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Dict/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2877 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Dict/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    12308 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/local/dictclient.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.676234 limnoria-2023.1.28/plugins/Dict/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3731 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3433 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3365 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6458 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2548 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dict/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Dunno/
--rw-r--r--   0 val       (1000) val       (1000)     2817 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2511 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Dunno/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1414 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1637 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1557 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1441 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3095 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3446 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Dunno/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Factoids/
--rw-r--r--   0 val       (1000) val       (1000)     2738 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4867 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Factoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14672 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    14207 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13986 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    37539 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10544 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Factoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Fediverse/
--rw-r--r--   0 val       (1000) val       (1000)     2506 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     9206 2023-02-11 09:15:12.000000 limnoria-2023.1.28/plugins/Fediverse/activitypub.py
--rw-r--r--   0 val       (1000) val       (1000)     3583 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/config.py
--rw-r--r--   0 val       (1000) val       (1000)    16631 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    21650 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/test.py
--rw-r--r--   0 val       (1000) val       (1000)    21570 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/test_data.py
--rw-r--r--   0 val       (1000) val       (1000)     2553 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Fediverse/utils.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Filter/
--rw-r--r--   0 val       (1000) val       (1000)     2691 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3118 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.680234 limnoria-2023.1.28/plugins/Filter/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14523 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13736 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    14301 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    27294 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7848 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Filter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/Format/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2522 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/Format/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6742 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5998 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6115 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7452 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4078 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Format/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/GPG/
--rw-r--r--   0 val       (1000) val       (1000)     2606 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/GPG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2996 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/GPG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     9566 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/GPG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5817 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/GPG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/Games/
--rw-r--r--   0 val       (1000) val       (1000)     2660 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2313 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/Games/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4801 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5274 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4968 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4732 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7248 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2854 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Games/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.684234 limnoria-2023.1.28/plugins/Geography/
--rw-r--r--   0 val       (1000) val       (1000)     2578 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1936 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/common.py
--rw-r--r--   0 val       (1000) val       (1000)     2441 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/config.py
--rw-r--r--   0 val       (1000) val       (1000)     2924 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/nominatim.py
--rw-r--r--   0 val       (1000) val       (1000)     6528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10114 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/test.py
--rw-r--r--   0 val       (1000) val       (1000)     5422 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Geography/wikidata.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.688234 limnoria-2023.1.28/plugins/Google/
--rw-r--r--   0 val       (1000) val       (1000)     2507 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     7042 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.688234 limnoria-2023.1.28/plugins/Google/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9595 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9003 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9000 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4460 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/parser.py
--rw-r--r--   0 val       (1000) val       (1000)    11693 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3095 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Google/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.688234 limnoria-2023.1.28/plugins/Hashes/
--rw-r--r--   0 val       (1000) val       (1000)     2585 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Hashes/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2244 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Hashes/config.py
--rw-r--r--   0 val       (1000) val       (1000)     4049 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Hashes/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2754 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Hashes/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.688234 limnoria-2023.1.28/plugins/Herald/
--rw-r--r--   0 val       (1000) val       (1000)     2423 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3907 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Herald/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7333 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6711 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6615 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10794 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Herald/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Internet/
--rw-r--r--   0 val       (1000) val       (1000)     2676 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Internet/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2313 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1791 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1769 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8887 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2420 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Internet/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Karma/
--rw-r--r--   0 val       (1000) val       (1000)     2540 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3929 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Karma/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7837 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7070 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7143 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    18303 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9962 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Karma/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Lart/
--rw-r--r--   0 val       (1000) val       (1000)     2571 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2679 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Lart/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2027 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1956 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4264 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2583 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Lart/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.692234 limnoria-2023.1.28/plugins/Later/
--rw-r--r--   0 val       (1000) val       (1000)     2650 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3413 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/Later/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7371 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7908 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6739 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7370 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11043 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6360 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Later/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/Limiter/
--rw-r--r--   0 val       (1000) val       (1000)     2662 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3141 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/Limiter/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2685 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2688 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2724 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2573 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3657 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2871 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Limiter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/LogToIrc/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/LogToIrc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5627 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/LogToIrc/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6213 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/LogToIrc/handler.py
--rw-r--r--   0 val       (1000) val       (1000)     2710 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/LogToIrc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1781 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/LogToIrc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/Math/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2516 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.696234 limnoria-2023.1.28/plugins/Math/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    46378 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/local/convertcore.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/Math/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5920 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5424 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5331 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5325 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11324 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9441 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Math/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/MessageParser/
--rw-r--r--   0 val       (1000) val       (1000)     3026 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4464 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/MessageParser/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11282 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10121 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10440 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20027 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    11653 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MessageParser/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/Misc/
--rw-r--r--   0 val       (1000) val       (1000)     2299 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4131 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/Misc/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13201 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    14554 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13747 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13209 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    13537 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    29646 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    17530 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Misc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.700235 limnoria-2023.1.28/plugins/MoobotFactoids/
--rw-r--r--   0 val       (1000) val       (1000)     2648 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2740 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/MoobotFactoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11225 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10014 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10059 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/locales/it.po
--rwxr-xr-x   0 val       (1000) val       (1000)    29418 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    16971 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/MoobotFactoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/Network/
--rw-r--r--   0 val       (1000) val       (1000)     2514 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/Network/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7181 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8612 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7289 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7472 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12616 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2008 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Network/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/News/
--rw-r--r--   0 val       (1000) val       (1000)     2777 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/News/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4608 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4221 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4314 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8659 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3616 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/News/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/NickAuth/
--rw-r--r--   0 val       (1000) val       (1000)     2574 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2495 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/NickAuth/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4837 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4838 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9213 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6306 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickAuth/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.704234 limnoria-2023.1.28/plugins/NickCapture/
--rw-r--r--   0 val       (1000) val       (1000)     2582 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2738 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/NickCapture/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1598 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1716 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1592 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1500 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     5415 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1799 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/NickCapture/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Nickometer/
--rw-r--r--   0 val       (1000) val       (1000)     3249 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2616 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Nickometer/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1338 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1027 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)      952 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9695 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2183 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Nickometer/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Note/
--rw-r--r--   0 val       (1000) val       (1000)     2645 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3477 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Note/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4033 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3453 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3399 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16493 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4040 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Note/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Owner/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3252 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.708234 limnoria-2023.1.28/plugins/Owner/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8724 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5600 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8546 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9038 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     8811 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    31629 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7618 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Owner/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/Plugin/
--rw-r--r--   0 val       (1000) val       (1000)     2666 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2523 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/Plugin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7234 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7937 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6377 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7290 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9985 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4272 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Plugin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/PluginDownloader/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2535 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/PluginDownloader/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4570 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6726 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6327 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5727 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16064 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3847 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/PluginDownloader/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/Poll/
--rw-r--r--   0 val       (1000) val       (1000)     2516 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Poll/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2922 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Poll/config.py
--rw-r--r--   0 val       (1000) val       (1000)     8542 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Poll/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6858 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Poll/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/Praise/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2695 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.712235 limnoria-2023.1.28/plugins/Praise/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2548 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2424 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2352 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4348 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1953 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Praise/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/Protector/
--rw-r--r--   0 val       (1000) val       (1000)     2594 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/Protector/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1626 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1245 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1153 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7598 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Protector/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/Quote/
--rw-r--r--   0 val       (1000) val       (1000)     2524 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/Quote/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1700 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1418 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1372 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3106 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Quote/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/QuoteGrabs/
--rw-r--r--   0 val       (1000) val       (1000)     2675 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3670 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/QuoteGrabs/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7337 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6529 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6636 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    17122 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8560 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/QuoteGrabs/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.716235 limnoria-2023.1.28/plugins/RSS/
--rw-r--r--   0 val       (1000) val       (1000)     2704 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6771 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.720234 limnoria-2023.1.28/plugins/RSS/locales/
--rw-r--r--   0 val       (1000) val       (1000)    12451 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    15597 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13213 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13001 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    12728 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    28159 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    19888 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/RSS/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.720234 limnoria-2023.1.28/plugins/Relay/
--rw-r--r--   0 val       (1000) val       (1000)     2517 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4744 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.720234 limnoria-2023.1.28/plugins/Relay/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8274 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7545 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7487 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19682 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Relay/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.720234 limnoria-2023.1.28/plugins/Reply/
--rw-r--r--   0 val       (1000) val       (1000)     2572 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.720234 limnoria-2023.1.28/plugins/Reply/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2384 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2630 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2331 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2669 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2433 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3694 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3051 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Reply/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/Scheduler/
--rw-r--r--   0 val       (1000) val       (1000)     2757 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Scheduler/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Scheduler/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/Scheduler/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4116 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Scheduler/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3797 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Scheduler/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3850 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Scheduler/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12852 2023-02-11 09:15:12.000000 limnoria-2023.1.28/plugins/Scheduler/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8402 2023-02-11 09:15:12.000000 limnoria-2023.1.28/plugins/Scheduler/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/SedRegex/
--rw-r--r--   0 val       (1000) val       (1000)     2709 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/SedRegex/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3524 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/SedRegex/config.py
--rwxr-xr-x   0 val       (1000) val       (1000)      874 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/SedRegex/constants.py
--rw-r--r--   0 val       (1000) val       (1000)    10335 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/SedRegex/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    12279 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/SedRegex/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/Seen/
--rw-r--r--   0 val       (1000) val       (1000)     2637 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/Seen/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5779 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6954 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6235 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5812 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15271 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5431 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Seen/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.724235 limnoria-2023.1.28/plugins/Services/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5658 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/Services/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11466 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    11843 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11294 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    11525 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    34301 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14436 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Services/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/ShrinkUrl/
--rw-r--r--   0 val       (1000) val       (1000)     2542 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5035 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/ShrinkUrl/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5983 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5213 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5243 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10186 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5286 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/ShrinkUrl/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/Status/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/Status/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5435 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6124 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5481 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5563 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10046 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3180 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Status/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/String/
--rw-r--r--   0 val       (1000) val       (1000)     2551 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3429 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.728235 limnoria-2023.1.28/plugins/String/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9469 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8780 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8557 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9858 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7585 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/String/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Success/
--rw-r--r--   0 val       (1000) val       (1000)     2646 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2751 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Success/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1578 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1435 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1323 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3471 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2272 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Success/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Time/
--rw-r--r--   0 val       (1000) val       (1000)     2673 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2640 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Time/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5480 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6313 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5483 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5849 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5574 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10127 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5071 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Time/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Todo/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2683 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.732235 limnoria-2023.1.28/plugins/Todo/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4575 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5089 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4595 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4664 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10596 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6654 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Todo/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/Topic/
--rw-r--r--   0 val       (1000) val       (1000)     2583 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4776 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/Topic/locales/
--rw-r--r--   0 val       (1000) val       (1000)    18502 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    16877 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    17231 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    25153 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13078 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Topic/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/URL/
--rw-r--r--   0 val       (1000) val       (1000)     2661 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2629 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/URL/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3421 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2907 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2841 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6765 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4241 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/URL/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/Unix/
--rw-r--r--   0 val       (1000) val       (1000)     2669 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6252 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/Unix/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13680 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11967 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    12075 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20048 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7736 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Unix/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/User/
--rw-r--r--   0 val       (1000) val       (1000)     2355 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2728 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.736235 limnoria-2023.1.28/plugins/User/locales/
--rw-r--r--   0 val       (1000) val       (1000)    15416 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    21068 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    19566 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10856 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    15349 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    23217 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9203 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/User/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.740235 limnoria-2023.1.28/plugins/Utilities/
--rw-r--r--   0 val       (1000) val       (1000)     2407 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.740235 limnoria-2023.1.28/plugins/Utilities/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3623 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4827 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4250 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4335 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7065 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3958 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Utilities/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.740235 limnoria-2023.1.28/plugins/Web/
--rw-r--r--   0 val       (1000) val       (1000)     2446 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5246 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.740235 limnoria-2023.1.28/plugins/Web/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7308 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8904 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7488 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7113 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16701 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9130 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/Web/test.py
--rw-r--r--   0 val       (1000) val       (1000)    23695 2023-02-11 09:14:15.000000 limnoria-2023.1.28/plugins/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)      192 2023-02-11 09:14:15.000000 limnoria-2023.1.28/pyproject.toml
--rw-r--r--   0 val       (1000) val       (1000)      866 2023-02-11 09:14:15.000000 limnoria-2023.1.28/requirements.txt
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.740235 limnoria-2023.1.28/scripts/
--rw-r--r--   0 val       (1000) val       (1000)    15833 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot
--rw-r--r--   0 val       (1000) val       (1000)     5258 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-adduser
--rw-r--r--   0 val       (1000) val       (1000)     5469 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-botchk
--rw-r--r--   0 val       (1000) val       (1000)    10510 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-plugin-create
--rw-r--r--   0 val       (1000) val       (1000)    14328 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-plugin-doc
--rw-r--r--   0 val       (1000) val       (1000)     4428 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-reset-password
--rw-r--r--   0 val       (1000) val       (1000)     9399 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-test
--rw-r--r--   0 val       (1000) val       (1000)    37678 2023-02-11 09:14:15.000000 limnoria-2023.1.28/scripts/supybot-wizard
--rw-r--r--   0 val       (1000) val       (1000)       38 2023-02-11 09:15:17.752235 limnoria-2023.1.28/setup.cfg
--rw-r--r--   0 val       (1000) val       (1000)     8575 2023-02-11 09:14:15.000000 limnoria-2023.1.28/setup.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.748235 limnoria-2023.1.28/src/
--rw-r--r--   0 val       (1000) val       (1000)     4117 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3548 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/ansi.py
--rw-r--r--   0 val       (1000) val       (1000)    74553 2023-02-11 09:15:12.000000 limnoria-2023.1.28/src/callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)    14986 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/cdb.py
--rw-r--r--   0 val       (1000) val       (1000)    41479 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/commands.py
--rw-r--r--   0 val       (1000) val       (1000)    66908 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/conf.py
--rw-r--r--   0 val       (1000) val       (1000)    14165 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/dbi.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.748235 limnoria-2023.1.28/src/drivers/
--rw-r--r--   0 val       (1000) val       (1000)    19096 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/drivers/Socket.py
--rw-r--r--   0 val       (1000) val       (1000)     9699 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/drivers/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2350 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     2997 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/gpg.py
--rw-r--r--   0 val       (1000) val       (1000)    17942 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/httpserver.py
--rw-r--r--   0 val       (1000) val       (1000)    13177 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    51899 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    97175 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    38939 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    43251 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)    16573 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/log.py
--rw-r--r--   0 val       (1000) val       (1000)     8379 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5342 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/questions.py
--rw-r--r--   0 val       (1000) val       (1000)    34261 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/registry.py
--rw-r--r--   0 val       (1000) val       (1000)     6156 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/schedule.py
--rw-r--r--   0 val       (1000) val       (1000)     4790 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/setup.py
--rw-r--r--   0 val       (1000) val       (1000)     8198 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/shlex.py
--rw-r--r--   0 val       (1000) val       (1000)    25444 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/test.py
--rw-r--r--   0 val       (1000) val       (1000)     3869 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/unpreserve.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.748235 limnoria-2023.1.28/src/utils/
--rw-r--r--   0 val       (1000) val       (1000)     2575 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1741 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/crypt.py
--rw-r--r--   0 val       (1000) val       (1000)     1992 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/error.py
--rw-r--r--   0 val       (1000) val       (1000)     9475 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/file.py
--rw-r--r--   0 val       (1000) val       (1000)    11587 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/gen.py
--rw-r--r--   0 val       (1000) val       (1000)     5210 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/iter.py
--rw-r--r--   0 val       (1000) val       (1000)     6195 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/math_evaluator.py
--rw-r--r--   0 val       (1000) val       (1000)     3914 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/minisix.py
--rw-r--r--   0 val       (1000) val       (1000)     6526 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/net.py
--rw-r--r--   0 val       (1000) val       (1000)     7726 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/python.py
--rw-r--r--   0 val       (1000) val       (1000)     4169 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/seq.py
--rw-r--r--   0 val       (1000) val       (1000)    21873 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/str.py
--rw-r--r--   0 val       (1000) val       (1000)    19840 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/structures.py
--rw-r--r--   0 val       (1000) val       (1000)     2838 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/time.py
--rw-r--r--   0 val       (1000) val       (1000)     8826 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/transaction.py
--rw-r--r--   0 val       (1000) val       (1000)    10662 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/utils/web.py
--rw-r--r--   0 val       (1000) val       (1000)      175 2023-02-11 09:15:17.000000 limnoria-2023.1.28/src/version.py
--rw-r--r--   0 val       (1000) val       (1000)     7660 2023-02-11 09:14:15.000000 limnoria-2023.1.28/src/world.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-02-11 09:15:17.752235 limnoria-2023.1.28/test/
--rw-r--r--   0 val       (1000) val       (1000)     1754 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2265 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test.py
--rw-r--r--   0 val       (1000) val       (1000)    48916 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)     9002 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_commands.py
--rw-r--r--   0 val       (1000) val       (1000)     2813 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_conf.py
--rw-r--r--   0 val       (1000) val       (1000)     4122 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_drivers.py
--rw-r--r--   0 val       (1000) val       (1000)     2458 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     3225 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_firewall.py
--rw-r--r--   0 val       (1000) val       (1000)     1925 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_format.py
--rw-r--r--   0 val       (1000) val       (1000)     2832 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    28459 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    67607 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    14083 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    22829 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)     3341 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_misc.py
--rw-r--r--   0 val       (1000) val       (1000)     2016 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4832 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_plugin_create.py
--rw-r--r--   0 val       (1000) val       (1000)     2430 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_plugins.py
--rw-r--r--   0 val       (1000) val       (1000)    13283 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_registry.py
--rw-r--r--   0 val       (1000) val       (1000)     4575 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_schedule.py
--rw-r--r--   0 val       (1000) val       (1000)     3759 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_standardSubstitute.py
--rw-r--r--   0 val       (1000) val       (1000)    49349 2023-02-11 09:14:15.000000 limnoria-2023.1.28/test/test_utils.py
--rw-r--r--   0 val       (1000) val       (1000)     3672 2023-02-11 09:15:12.000000 limnoria-2023.1.28/test/test_yn.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.502385 limnoria-2023.4.28/
+-rw-r--r--   0 val       (1000) val       (1000)     1654 2023-05-18 13:06:04.000000 limnoria-2023.4.28/LICENSE.md
+-rw-r--r--   0 val       (1000) val       (1000)      117 2023-05-18 13:06:04.000000 limnoria-2023.4.28/MANIFEST.in
+-rw-r--r--   0 val       (1000) val       (1000)      983 2023-05-18 13:06:04.000000 limnoria-2023.4.28/Makefile
+-rw-r--r--   0 val       (1000) val       (1000)     1746 2023-05-18 13:06:35.498385 limnoria-2023.4.28/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)     2292 2023-05-18 13:06:04.000000 limnoria-2023.4.28/README.md
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/limnoria.egg-info/
+-rw-r--r--   0 val       (1000) val       (1000)     1746 2023-05-18 13:06:35.000000 limnoria-2023.4.28/limnoria.egg-info/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)    16256 2023-05-18 13:06:35.000000 limnoria-2023.4.28/limnoria.egg-info/SOURCES.txt
+-rw-r--r--   0 val       (1000) val       (1000)        1 2023-05-18 13:06:35.000000 limnoria-2023.4.28/limnoria.egg-info/dependency_links.txt
+-rw-r--r--   0 val       (1000) val       (1000)      934 2023-05-18 13:06:35.000000 limnoria-2023.4.28/limnoria.egg-info/entry_points.txt
+-rw-r--r--   0 val       (1000) val       (1000)        8 2023-05-18 13:06:35.000000 limnoria-2023.4.28/limnoria.egg-info/top_level.txt
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/locales/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    54113 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    76337 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    77441 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3749 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/fr.py
+-rw-r--r--   0 val       (1000) val       (1000)    69991 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    42399 2023-05-18 13:06:04.000000 limnoria-2023.4.28/locales/messages.pot
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/man/
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/limnoria.1
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2023-05-18 13:06:27.000000 limnoria-2023.4.28/man/supybot.1
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/Admin/
+-rw-r--r--   0 val       (1000) val       (1000)     2422 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2312 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/Admin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8064 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8857 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7809 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8112 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15152 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5897 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Admin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/Aka/
+-rw-r--r--   0 val       (1000) val       (1000)     2788 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Aka/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Aka/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/Aka/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11022 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Aka/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    39586 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Aka/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14785 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Aka/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.454385 limnoria-2023.4.28/plugins/Alias/
+-rw-r--r--   0 val       (1000) val       (1000)     2655 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2539 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Alias/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4716 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5751 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5059 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5176 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     4919 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19130 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8039 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Alias/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Anonymous/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3516 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Anonymous/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6558 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7384 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5903 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6893 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     6535 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9054 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6882 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Anonymous/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/AutoMode/
+-rw-r--r--   0 val       (1000) val       (1000)     2697 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4521 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/AutoMode/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4202 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5058 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4512 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8029 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/AutoMode/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Autocomplete/
+-rw-r--r--   0 val       (1000) val       (1000)     2946 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Autocomplete/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2808 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Autocomplete/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6158 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Autocomplete/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6635 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Autocomplete/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/BadWords/
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6163 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/BadWords/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6862 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6112 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6277 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7475 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3943 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/BadWords/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Channel/
+-rw-r--r--   0 val       (1000) val       (1000)     2480 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3497 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/Channel/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    32456 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    35277 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    32166 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    32899 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    33333 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    44412 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13344 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Channel/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/ChannelLogger/
+-rw-r--r--   0 val       (1000) val       (1000)     2531 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5994 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/ChannelLogger/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5491 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5340 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5607 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5183 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    13745 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9242 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelLogger/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.458385 limnoria-2023.4.28/plugins/ChannelStats/
+-rw-r--r--   0 val       (1000) val       (1000)     2682 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3449 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/ChannelStats/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6426 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6640 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6242 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15391 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4870 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ChannelStats/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Conditional/
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2763 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Conditional/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8160 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7180 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7493 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11342 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6497 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Conditional/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Config/
+-rw-r--r--   0 val       (1000) val       (1000)     2325 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Config/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9209 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     9329 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     9265 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    21747 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    25531 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Config/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Ctcp/
+-rw-r--r--   0 val       (1000) val       (1000)     2420 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3652 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Ctcp/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2084 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2196 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2072 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2073 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     1911 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7136 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1785 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Ctcp/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/DDG/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/DDG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3332 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/DDG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6037 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/DDG/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)     6988 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/DDG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2389 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/DDG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Debug/
+-rw-r--r--   0 val       (1000) val       (1000)     2377 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Debug/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2399 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Debug/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     7272 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Debug/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Debug/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Dict/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2877 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Dict/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    12308 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/local/dictclient.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Dict/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3731 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3433 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3365 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6458 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dict/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Dunno/
+-rw-r--r--   0 val       (1000) val       (1000)     2817 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2511 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Dunno/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1414 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1637 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1557 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1441 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3446 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Dunno/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.462385 limnoria-2023.4.28/plugins/Factoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4867 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Factoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14672 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    14207 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13986 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    37539 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10544 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Factoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Fediverse/
+-rw-r--r--   0 val       (1000) val       (1000)     2506 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     9206 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/activitypub.py
+-rw-r--r--   0 val       (1000) val       (1000)     3583 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/config.py
+-rw-r--r--   0 val       (1000) val       (1000)    16631 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    21650 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    21570 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/test_data.py
+-rw-r--r--   0 val       (1000) val       (1000)     2553 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Fediverse/utils.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Filter/
+-rw-r--r--   0 val       (1000) val       (1000)     2691 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3118 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Filter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14523 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13736 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    14301 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    27294 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7848 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Filter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Format/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2522 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Format/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6742 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5998 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6115 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7452 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4078 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Format/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/GPG/
+-rw-r--r--   0 val       (1000) val       (1000)     2606 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/GPG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2996 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/GPG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     9566 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/GPG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5817 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/GPG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Games/
+-rw-r--r--   0 val       (1000) val       (1000)     2660 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Games/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4801 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5274 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4968 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4732 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7248 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2854 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Games/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Geography/
+-rw-r--r--   0 val       (1000) val       (1000)     2578 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1936 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/common.py
+-rw-r--r--   0 val       (1000) val       (1000)     2441 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     2924 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/nominatim.py
+-rw-r--r--   0 val       (1000) val       (1000)     6528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10114 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     5422 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Geography/wikidata.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Google/
+-rw-r--r--   0 val       (1000) val       (1000)     2507 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     7042 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Google/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9595 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9003 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9000 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4460 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)    11693 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Google/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.466385 limnoria-2023.4.28/plugins/Hashes/
+-rw-r--r--   0 val       (1000) val       (1000)     2585 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Hashes/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2244 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Hashes/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     4049 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Hashes/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2754 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Hashes/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Herald/
+-rw-r--r--   0 val       (1000) val       (1000)     2423 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3907 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Herald/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7333 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6711 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6615 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10794 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Herald/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Internet/
+-rw-r--r--   0 val       (1000) val       (1000)     2676 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Internet/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1791 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1769 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8887 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2420 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Internet/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Karma/
+-rw-r--r--   0 val       (1000) val       (1000)     2540 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3929 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Karma/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7837 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7070 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7143 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    18303 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9962 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Karma/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Lart/
+-rw-r--r--   0 val       (1000) val       (1000)     2571 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2679 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Lart/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2027 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1956 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4264 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Lart/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Later/
+-rw-r--r--   0 val       (1000) val       (1000)     2650 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3413 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Later/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7371 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7908 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6739 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7370 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11043 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6360 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Later/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Limiter/
+-rw-r--r--   0 val       (1000) val       (1000)     2662 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3141 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/Limiter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2685 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2688 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2724 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2573 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3657 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2871 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Limiter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.470385 limnoria-2023.4.28/plugins/LogToIrc/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/LogToIrc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5627 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/LogToIrc/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6213 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/LogToIrc/handler.py
+-rw-r--r--   0 val       (1000) val       (1000)     2710 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/LogToIrc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1781 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/LogToIrc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Math/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Math/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    46378 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/local/convertcore.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Math/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5920 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5424 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5331 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5325 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11324 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9441 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Math/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/MessageParser/
+-rw-r--r--   0 val       (1000) val       (1000)     3026 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4464 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/MessageParser/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11282 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10121 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10440 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20027 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    11653 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MessageParser/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Misc/
+-rw-r--r--   0 val       (1000) val       (1000)     2299 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Misc/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13201 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    14554 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13747 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13209 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    13537 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    29646 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    17530 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Misc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/MoobotFactoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2740 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/MoobotFactoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11225 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10014 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10059 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/locales/it.po
+-rwxr-xr-x   0 val       (1000) val       (1000)    29418 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    16971 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/MoobotFactoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.474385 limnoria-2023.4.28/plugins/Network/
+-rw-r--r--   0 val       (1000) val       (1000)     2514 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Network/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7181 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8612 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7289 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7472 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12616 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2008 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Network/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/News/
+-rw-r--r--   0 val       (1000) val       (1000)     2777 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/News/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4608 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4221 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4314 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8659 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3616 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/News/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/NickAuth/
+-rw-r--r--   0 val       (1000) val       (1000)     2574 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2495 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/NickAuth/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4837 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4838 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9213 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6306 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickAuth/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/NickCapture/
+-rw-r--r--   0 val       (1000) val       (1000)     2582 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/NickCapture/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1598 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1716 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1592 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1500 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     5415 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1799 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/NickCapture/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Nickometer/
+-rw-r--r--   0 val       (1000) val       (1000)     3249 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2616 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Nickometer/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1338 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1027 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)      952 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9695 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2183 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Nickometer/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Note/
+-rw-r--r--   0 val       (1000) val       (1000)     2645 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3477 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Note/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4033 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3453 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3399 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16493 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4040 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Note/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Owner/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3252 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Owner/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8724 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5600 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8546 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9038 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     8811 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    31629 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7618 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Owner/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.478385 limnoria-2023.4.28/plugins/Plugin/
+-rw-r--r--   0 val       (1000) val       (1000)     2666 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2523 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Plugin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7234 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7937 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6377 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7290 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9985 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4272 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Plugin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/PluginDownloader/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2535 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/PluginDownloader/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4570 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6726 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6327 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5727 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16064 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3847 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/PluginDownloader/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Poll/
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Poll/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2922 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Poll/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     8542 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Poll/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6858 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Poll/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Praise/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Praise/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2424 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2352 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4348 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1953 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Praise/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Protector/
+-rw-r--r--   0 val       (1000) val       (1000)     2594 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Protector/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1626 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1245 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1153 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7598 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Protector/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Quote/
+-rw-r--r--   0 val       (1000) val       (1000)     2524 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/Quote/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1700 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1418 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1372 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3106 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Quote/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/QuoteGrabs/
+-rw-r--r--   0 val       (1000) val       (1000)     2675 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3670 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/QuoteGrabs/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7337 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6529 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6636 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    17122 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8560 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/QuoteGrabs/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/RSS/
+-rw-r--r--   0 val       (1000) val       (1000)     2704 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6771 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.482385 limnoria-2023.4.28/plugins/RSS/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    12451 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    15597 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13213 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13001 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    12728 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    28159 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    19888 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/RSS/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Relay/
+-rw-r--r--   0 val       (1000) val       (1000)     2517 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4744 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Relay/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8274 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7545 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7487 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19682 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Relay/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Reply/
+-rw-r--r--   0 val       (1000) val       (1000)     2572 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Reply/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2384 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2630 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2331 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2433 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3694 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3051 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Reply/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Scheduler/
+-rw-r--r--   0 val       (1000) val       (1000)     2757 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Scheduler/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4116 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3797 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3850 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12852 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8402 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Scheduler/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/SedRegex/
+-rw-r--r--   0 val       (1000) val       (1000)     2709 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/SedRegex/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3524 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/SedRegex/config.py
+-rwxr-xr-x   0 val       (1000) val       (1000)      874 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/SedRegex/constants.py
+-rw-r--r--   0 val       (1000) val       (1000)    10335 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/SedRegex/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    12279 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/SedRegex/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Seen/
+-rw-r--r--   0 val       (1000) val       (1000)     2637 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Seen/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5779 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6954 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6235 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5812 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15271 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5431 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Seen/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Services/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5658 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Services/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11466 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    11843 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11294 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    11525 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    34301 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14436 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Services/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/ShrinkUrl/
+-rw-r--r--   0 val       (1000) val       (1000)     2542 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5035 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/ShrinkUrl/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5983 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5213 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5243 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10186 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5286 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/ShrinkUrl/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Status/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.486384 limnoria-2023.4.28/plugins/Status/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5435 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6124 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5481 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5563 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10046 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3180 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Status/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/String/
+-rw-r--r--   0 val       (1000) val       (1000)     2551 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3429 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/String/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9469 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8780 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8557 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9858 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7585 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/String/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Success/
+-rw-r--r--   0 val       (1000) val       (1000)     2646 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2751 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Success/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1578 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1435 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1323 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3471 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2272 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Success/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Time/
+-rw-r--r--   0 val       (1000) val       (1000)     2673 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2640 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Time/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5480 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6313 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5483 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5849 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5574 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10127 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5071 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Time/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Todo/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2683 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Todo/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5089 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4595 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4664 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10596 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6654 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Todo/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Topic/
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4776 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Topic/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    18502 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    16877 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    17231 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    25153 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13078 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Topic/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/URL/
+-rw-r--r--   0 val       (1000) val       (1000)     2661 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2629 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/URL/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3421 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2841 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6765 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4241 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/URL/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Unix/
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6252 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/Unix/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13680 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11967 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    12075 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20048 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7736 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Unix/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.490385 limnoria-2023.4.28/plugins/User/
+-rw-r--r--   0 val       (1000) val       (1000)     2355 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2728 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.494385 limnoria-2023.4.28/plugins/User/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    15416 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    21068 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    19566 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10856 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    15349 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    23217 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9203 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/User/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.494385 limnoria-2023.4.28/plugins/Utilities/
+-rw-r--r--   0 val       (1000) val       (1000)     2407 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.494385 limnoria-2023.4.28/plugins/Utilities/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3623 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4827 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4250 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4335 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7065 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3958 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Utilities/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.494385 limnoria-2023.4.28/plugins/Web/
+-rw-r--r--   0 val       (1000) val       (1000)     2446 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5246 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.494385 limnoria-2023.4.28/plugins/Web/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7308 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8904 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7488 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7113 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16701 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9130 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/Web/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    23695 2023-05-18 13:06:04.000000 limnoria-2023.4.28/plugins/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)      192 2023-05-18 13:06:04.000000 limnoria-2023.4.28/pyproject.toml
+-rw-r--r--   0 val       (1000) val       (1000)      866 2023-05-18 13:06:04.000000 limnoria-2023.4.28/requirements.txt
+-rw-r--r--   0 val       (1000) val       (1000)       38 2023-05-18 13:06:35.502385 limnoria-2023.4.28/setup.cfg
+-rw-r--r--   0 val       (1000) val       (1000)     8346 2023-05-18 13:06:27.000000 limnoria-2023.4.28/setup.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.498385 limnoria-2023.4.28/src/
+-rw-r--r--   0 val       (1000) val       (1000)     4117 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3548 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/ansi.py
+-rw-r--r--   0 val       (1000) val       (1000)    74553 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)    14986 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/cdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    41479 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/commands.py
+-rw-r--r--   0 val       (1000) val       (1000)    66908 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/conf.py
+-rw-r--r--   0 val       (1000) val       (1000)    14165 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/dbi.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.498385 limnoria-2023.4.28/src/drivers/
+-rw-r--r--   0 val       (1000) val       (1000)    19096 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/drivers/Socket.py
+-rw-r--r--   0 val       (1000) val       (1000)     9699 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/drivers/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2350 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     2997 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/gpg.py
+-rw-r--r--   0 val       (1000) val       (1000)    17942 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/httpserver.py
+-rw-r--r--   0 val       (1000) val       (1000)    13177 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    51899 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    97203 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    38939 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    43251 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)    16573 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/log.py
+-rw-r--r--   0 val       (1000) val       (1000)     8379 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5342 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/questions.py
+-rw-r--r--   0 val       (1000) val       (1000)    34261 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     6156 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/schedule.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.498385 limnoria-2023.4.28/src/scripts/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    15886 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria.py
+-rw-r--r--   0 val       (1000) val       (1000)     5258 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_adduser.py
+-rw-r--r--   0 val       (1000) val       (1000)     5493 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_botchk.py
+-rw-r--r--   0 val       (1000) val       (1000)    10536 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)    14353 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_plugin_doc.py
+-rw-r--r--   0 val       (1000) val       (1000)     4453 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_reset_password.py
+-rw-r--r--   0 val       (1000) val       (1000)     9424 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_test.py
+-rw-r--r--   0 val       (1000) val       (1000)    37705 2023-05-18 13:06:27.000000 limnoria-2023.4.28/src/scripts/limnoria_wizard.py
+-rw-r--r--   0 val       (1000) val       (1000)     4790 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/setup.py
+-rw-r--r--   0 val       (1000) val       (1000)     8198 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/shlex.py
+-rw-r--r--   0 val       (1000) val       (1000)    25444 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     3869 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/unpreserve.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.498385 limnoria-2023.4.28/src/utils/
+-rw-r--r--   0 val       (1000) val       (1000)     2575 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1741 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/crypt.py
+-rw-r--r--   0 val       (1000) val       (1000)     1992 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/error.py
+-rw-r--r--   0 val       (1000) val       (1000)     9475 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/file.py
+-rw-r--r--   0 val       (1000) val       (1000)    11587 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/gen.py
+-rw-r--r--   0 val       (1000) val       (1000)     5210 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/iter.py
+-rw-r--r--   0 val       (1000) val       (1000)     6195 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/math_evaluator.py
+-rw-r--r--   0 val       (1000) val       (1000)     3914 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/minisix.py
+-rw-r--r--   0 val       (1000) val       (1000)     6526 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/net.py
+-rw-r--r--   0 val       (1000) val       (1000)     7726 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/python.py
+-rw-r--r--   0 val       (1000) val       (1000)     4169 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/seq.py
+-rw-r--r--   0 val       (1000) val       (1000)    21873 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/str.py
+-rw-r--r--   0 val       (1000) val       (1000)    19840 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/structures.py
+-rw-r--r--   0 val       (1000) val       (1000)     2838 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/time.py
+-rw-r--r--   0 val       (1000) val       (1000)     8826 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/transaction.py
+-rw-r--r--   0 val       (1000) val       (1000)    10662 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/utils/web.py
+-rw-r--r--   0 val       (1000) val       (1000)      175 2023-05-18 13:06:35.000000 limnoria-2023.4.28/src/version.py
+-rw-r--r--   0 val       (1000) val       (1000)     7660 2023-05-18 13:06:04.000000 limnoria-2023.4.28/src/world.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-05-18 13:06:35.498385 limnoria-2023.4.28/test/
+-rw-r--r--   0 val       (1000) val       (1000)     1754 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2265 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    48916 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)     9002 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_commands.py
+-rw-r--r--   0 val       (1000) val       (1000)     2813 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_conf.py
+-rw-r--r--   0 val       (1000) val       (1000)     4122 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_drivers.py
+-rw-r--r--   0 val       (1000) val       (1000)     2458 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     3225 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_firewall.py
+-rw-r--r--   0 val       (1000) val       (1000)     1925 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_format.py
+-rw-r--r--   0 val       (1000) val       (1000)     2832 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    28459 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    67607 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    14083 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    22829 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3341 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_misc.py
+-rw-r--r--   0 val       (1000) val       (1000)     2016 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4832 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)     2430 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_plugins.py
+-rw-r--r--   0 val       (1000) val       (1000)    13283 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_schedule.py
+-rw-r--r--   0 val       (1000) val       (1000)     3759 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_standardSubstitute.py
+-rw-r--r--   0 val       (1000) val       (1000)    49349 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_utils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3672 2023-05-18 13:06:04.000000 limnoria-2023.4.28/test/test_yn.py
```

### Comparing `limnoria-2023.1.28/LICENSE.md` & `limnoria-2023.4.28/LICENSE.md`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/Makefile` & `limnoria-2023.4.28/Makefile`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/PKG-INFO` & `limnoria-2023.4.28/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2023.1.28
+Version: 2023.4.28
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
+Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
-License: UNKNOWN
-Download-URL: https://pypi.python.org/pypi/limnoria
 Platform: linux
 Platform: linux2
 Platform: win32
 Platform: cygwin
 Platform: darwin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -33,8 +32,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides: supybot
 License-File: LICENSE.md
 
 A robust, full-featured Python IRC bot with a clean and flexible plugin API. Equipped with a complete ACL system for specifying user permissions with as much as per-command granularity. Batteries are included in the form of numerous plugins already written.
-
```

### Comparing `limnoria-2023.1.28/README.md` & `limnoria-2023.4.28/README.md`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/limnoria.egg-info/PKG-INFO` & `limnoria-2023.4.28/limnoria.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2023.1.28
+Version: 2023.4.28
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
+Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
-License: UNKNOWN
-Download-URL: https://pypi.python.org/pypi/limnoria
 Platform: linux
 Platform: linux2
 Platform: win32
 Platform: cygwin
 Platform: darwin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -33,8 +32,7 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides: supybot
 License-File: LICENSE.md
 
 A robust, full-featured Python IRC bot with a clean and flexible plugin API. Equipped with a complete ACL system for specifying user permissions with as much as per-command granularity. Batteries are included in the form of numerous plugins already written.
-
```

### Comparing `limnoria-2023.1.28/limnoria.egg-info/SOURCES.txt` & `limnoria-2023.4.28/limnoria.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 limnoria.egg-info/PKG-INFO
 limnoria.egg-info/SOURCES.txt
 limnoria.egg-info/dependency_links.txt
+limnoria.egg-info/entry_points.txt
 limnoria.egg-info/top_level.txt
 locales/__init__.py
 locales/de.po
 locales/fi.po
 locales/fr.po
 locales/fr.py
 locales/it.po
 locales/messages.pot
+man/limnoria-adduser.1
+man/limnoria-botchk.1
+man/limnoria-plugin-create.1
+man/limnoria-plugin-doc.1
+man/limnoria-reset-password.1
+man/limnoria-test.1
+man/limnoria-wizard.1
+man/limnoria.1
 man/supybot-adduser.1
 man/supybot-botchk.1
 man/supybot-plugin-create.1
 man/supybot-plugin-doc.1
 man/supybot-reset-password.1
 man/supybot-test.1
 man/supybot-wizard.1
@@ -532,22 +541,14 @@
 plugins/Web/config.py
 plugins/Web/plugin.py
 plugins/Web/test.py
 plugins/Web/locales/de.po
 plugins/Web/locales/fi.po
 plugins/Web/locales/fr.po
 plugins/Web/locales/it.po
-scripts/supybot
-scripts/supybot-adduser
-scripts/supybot-botchk
-scripts/supybot-plugin-create
-scripts/supybot-plugin-doc
-scripts/supybot-reset-password
-scripts/supybot-test
-scripts/supybot-wizard
 src/__init__.py
 src/ansi.py
 src/callbacks.py
 src/cdb.py
 src/commands.py
 src/conf.py
 src/dbi.py
@@ -568,14 +569,23 @@
 src/shlex.py
 src/test.py
 src/unpreserve.py
 src/version.py
 src/world.py
 src/drivers/Socket.py
 src/drivers/__init__.py
+src/scripts/__init__.py
+src/scripts/limnoria.py
+src/scripts/limnoria_adduser.py
+src/scripts/limnoria_botchk.py
+src/scripts/limnoria_plugin_create.py
+src/scripts/limnoria_plugin_doc.py
+src/scripts/limnoria_reset_password.py
+src/scripts/limnoria_test.py
+src/scripts/limnoria_wizard.py
 src/utils/__init__.py
 src/utils/crypt.py
 src/utils/error.py
 src/utils/file.py
 src/utils/gen.py
 src/utils/iter.py
 src/utils/math_evaluator.py
```

### Comparing `limnoria-2023.1.28/locales/de.po` & `limnoria-2023.4.28/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/locales/fi.po` & `limnoria-2023.4.28/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/locales/fr.po` & `limnoria-2023.4.28/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/locales/fr.py` & `limnoria-2023.4.28/locales/fr.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/locales/it.po` & `limnoria-2023.4.28/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/locales/messages.pot` & `limnoria-2023.4.28/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/man/supybot-adduser.1` & `limnoria-2023.4.28/man/limnoria-adduser.1`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .\" Process this file with
-.\" groff -man -Tascii supybot-adduser.1
+.\" groff -man -Tascii limnoria-adduser.1
 .\"
-.TH SUPYBOT-ADDUSER 1 "APRIL 2005"
+.TH LIMNORIA-ADDUSER 1 "APRIL 2005"
 .SH NAME
-supybot-adduser \- Adds a user to a Supybot users.conf file
+limnoria-adduser \- Adds a user to a Limnoria users.conf file
 .SH SYNOPSIS
-.B supybot-adduser
+.B limnoria-adduser
 .RI [ options ] " users.conf
 .SH DESCRIPTION
-.B supybot-adduser
+.B limnoria-adduser
 adds a user to the specified users.conf file.
 .SH OPTIONS
 .TP
 .B \-\^\-version
 Show version of program.
 .TP
 .BR \-h ", " \-\^\-help
@@ -25,18 +25,18 @@
 Specifies the password to use for the new user.
 .TP
 .BR \-c " CAPABILITY" "\fR,\fP \-\^\-capability=" CAPABILITY
 Capability the user should have; this option may be given
 multiple times.
 .SH "SEE ALSO"
 .IR python (1),
-.IR supybot (1),
-.IR supybot-test (1),
-.IR supybot-botchk (1),
-.IR supybot-wizard (1),
-.IR supybot-plugin-doc (1),
-.IR supybot-plugin-create (1)
+.IR limnoria (1),
+.IR limnoria-test (1),
+.IR limnoria-botchk (1),
+.IR limnoria-wizard (1),
+.IR limnoria-plugin-doc (1),
+.IR limnoria-plugin-create (1)
 .SH AUTHOR
 This manual page was originally written by James McCoy
 <vega dot james at gmail dot com>.  Permission is granted to copy,
-distribute and/or modify this document under the terms of the Supybot
+distribute and/or modify this document under the terms of the Limnoria
 license, a BSD-style license.
```

### Comparing `limnoria-2023.1.28/man/supybot-plugin-create.1` & `limnoria-2023.4.28/man/limnoria-plugin-create.1`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .\" Process this file with
-.\" groff -man -Tascii supybot-plugin-create.1
+.\" groff -man -Tascii limnoria-plugin-create.1
 .\"
-.TH SUPYBOT-PLUGIN-CREATE 1 "APRIL 2005"
+.TH LIMNORIA-PLUGIN-CREATE 1 "APRIL 2005"
 .SH NAME
-supybot-plugin-create \- A wizard for creating Supybot plugins
+limnoria-plugin-create \- A wizard for creating Limnoria plugins
 .SH SYNOPSIS
-.B supybot-plugin-create
+.B limnoria-plugin-create
 .RI [ options ]
 .SH DESCRIPTION
-.B supybot-plugin-create
+.B limnoria-plugin-create
 is a wizard that creates a template python source file for a new
-.IR supybot (1)
+.IR limnoria (1)
 plugin.
 .SH OPTIONS
 .TP
 .B \-\^\-version
 Show version of program.
 .TP
 .BR \-h ", " \-\^\-help
@@ -26,18 +26,18 @@
 .BR \-t ", " \-\^\-thread
 Makes the plugin threaded.
 .TP
 .BI \-\^\-real\-name= REALNAME
 Specify what real name the copyright is assigned to.
 .SH "SEE ALSO"
 .IR python (1),
-.IR supybot (1),
-.IR supybot-test (1),
-.IR supybot-botchk (1),
-.IR supybot-wizard (1),
-.IR supybot-adduser (1),
-.IR supybot-plugin-doc (1)
+.IR limnoria (1),
+.IR limnoria-test (1),
+.IR limnoria-botchk (1),
+.IR limnoria-wizard (1),
+.IR limnoria-adduser (1),
+.IR limnoria-plugin-doc (1)
 .SH AUTHOR
 This manual page was originally written by James McCoy
 <vega dot james at gmail dot com>.  Permission is granted to copy,
-distribute and/or modify this document under the terms of the Supybot
+distribute and/or modify this document under the terms of the Limnoria
 license, a BSD-style license.
```

### Comparing `limnoria-2023.1.28/man/supybot.1` & `limnoria-2023.4.28/man/limnoria.1`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .\" Process this file with
-.\" groff -man -Tascii supybot.1
+.\" groff -man -Tascii limnoria.1
 .\"
-.TH SUPYBOT 1 "JULY 2009"
+.TH LIMNORIA 1 "JULY 2009"
 .SH NAME
-supybot - A robust and user friendly Python IRC bot
+limnoria - A robust and user friendly Python IRC bot
 .SH SYNOPSIS
-.B supybot
+.B limnoria
 .RI [ options ] " configFile
 .SH DESCRIPTION
-.B Supybot
+.B Limnoria
 is a robust, user-friendly, and programmer-friendly Python IRC bot.
 It aims to be an adequate replacement for most existing IRC bots.  It
 includes a very flexible and powerful ACL system for controlling access
 to commands, as well as more than 50 builtin plugins providing around
 400 actual commands.
 .SH OPTIONS
 .TP
@@ -49,18 +49,18 @@
 want this.  Do not do it.  Even if you think you want it, you do not.
 .TP
 .B \-\^\-debug
 Determines whether some extra debugging stuff will be logged by this
 script.
 .SH "SEE ALSO"
 .IR python (1),
-.IR supybot-test (1),
-.IR supybot-botchk (1),
-.IR supybot-wizard (1),
-.IR supybot-adduser (1),
-.IR supybot-plugin-doc (1),
-.IR supybot-plugin-create (1)
+.IR limnoria-test (1),
+.IR limnoria-botchk (1),
+.IR limnoria-wizard (1),
+.IR limnoria-adduser (1),
+.IR limnoria-plugin-doc (1),
+.IR limnoria-plugin-create (1)
 .SH AUTHOR
 This manual page was originally written by James McCoy
 <vega dot james at gmail dot com>.  Permission is granted to copy,
-distribute and/or modify this document under the terms of the Supybot
+distribute and/or modify this document under the terms of the Limnoria
 license, a BSD-style license.
```

### Comparing `limnoria-2023.1.28/plugins/Admin/__init__.py` & `limnoria-2023.4.28/plugins/Admin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/config.py` & `limnoria-2023.4.28/plugins/Admin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/locales/de.po` & `limnoria-2023.4.28/plugins/Admin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/locales/fi.po` & `limnoria-2023.4.28/plugins/Admin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/locales/fr.po` & `limnoria-2023.4.28/plugins/Admin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/locales/it.po` & `limnoria-2023.4.28/plugins/Admin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/plugin.py` & `limnoria-2023.4.28/plugins/Admin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Admin/test.py` & `limnoria-2023.4.28/plugins/Admin/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Aka/__init__.py` & `limnoria-2023.4.28/plugins/Aka/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Aka/config.py` & `limnoria-2023.4.28/plugins/Aka/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Aka/locales/fi.po` & `limnoria-2023.4.28/plugins/Aka/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Aka/plugin.py` & `limnoria-2023.4.28/plugins/Aka/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Aka/test.py` & `limnoria-2023.4.28/plugins/Aka/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/__init__.py` & `limnoria-2023.4.28/plugins/Alias/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/config.py` & `limnoria-2023.4.28/plugins/Alias/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/locales/de.po` & `limnoria-2023.4.28/plugins/Alias/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/locales/fi.po` & `limnoria-2023.4.28/plugins/Alias/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/locales/fr.po` & `limnoria-2023.4.28/plugins/Alias/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/locales/hu.po` & `limnoria-2023.4.28/plugins/Alias/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/locales/it.po` & `limnoria-2023.4.28/plugins/Alias/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/plugin.py` & `limnoria-2023.4.28/plugins/Alias/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Alias/test.py` & `limnoria-2023.4.28/plugins/Alias/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/__init__.py` & `limnoria-2023.4.28/plugins/Anonymous/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/config.py` & `limnoria-2023.4.28/plugins/Anonymous/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/locales/de.po` & `limnoria-2023.4.28/plugins/Anonymous/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/locales/fi.po` & `limnoria-2023.4.28/plugins/Anonymous/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/locales/fr.po` & `limnoria-2023.4.28/plugins/Anonymous/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/locales/hu.po` & `limnoria-2023.4.28/plugins/Anonymous/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/locales/it.po` & `limnoria-2023.4.28/plugins/Anonymous/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/plugin.py` & `limnoria-2023.4.28/plugins/Anonymous/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Anonymous/test.py` & `limnoria-2023.4.28/plugins/Anonymous/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/__init__.py` & `limnoria-2023.4.28/plugins/AutoMode/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/config.py` & `limnoria-2023.4.28/plugins/AutoMode/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/locales/de.po` & `limnoria-2023.4.28/plugins/AutoMode/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/locales/fi.po` & `limnoria-2023.4.28/plugins/AutoMode/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/locales/fr.po` & `limnoria-2023.4.28/plugins/AutoMode/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/locales/it.po` & `limnoria-2023.4.28/plugins/AutoMode/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/plugin.py` & `limnoria-2023.4.28/plugins/AutoMode/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/AutoMode/test.py` & `limnoria-2023.4.28/plugins/AutoMode/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Autocomplete/__init__.py` & `limnoria-2023.4.28/plugins/Autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Autocomplete/config.py` & `limnoria-2023.4.28/plugins/Autocomplete/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Autocomplete/plugin.py` & `limnoria-2023.4.28/plugins/Autocomplete/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Autocomplete/test.py` & `limnoria-2023.4.28/plugins/Autocomplete/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/__init__.py` & `limnoria-2023.4.28/plugins/BadWords/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/config.py` & `limnoria-2023.4.28/plugins/BadWords/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/locales/fi.po` & `limnoria-2023.4.28/plugins/BadWords/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/locales/fr.po` & `limnoria-2023.4.28/plugins/BadWords/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/locales/it.po` & `limnoria-2023.4.28/plugins/BadWords/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/plugin.py` & `limnoria-2023.4.28/plugins/BadWords/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/BadWords/test.py` & `limnoria-2023.4.28/plugins/BadWords/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/__init__.py` & `limnoria-2023.4.28/plugins/Channel/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/config.py` & `limnoria-2023.4.28/plugins/Channel/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/locales/de.po` & `limnoria-2023.4.28/plugins/Channel/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/locales/fi.po` & `limnoria-2023.4.28/plugins/Channel/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/locales/fr.po` & `limnoria-2023.4.28/plugins/Channel/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/locales/hu.po` & `limnoria-2023.4.28/plugins/Channel/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/locales/it.po` & `limnoria-2023.4.28/plugins/Channel/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/plugin.py` & `limnoria-2023.4.28/plugins/Channel/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Channel/test.py` & `limnoria-2023.4.28/plugins/Channel/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/__init__.py` & `limnoria-2023.4.28/plugins/ChannelLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/config.py` & `limnoria-2023.4.28/plugins/ChannelLogger/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/locales/fi.po` & `limnoria-2023.4.28/plugins/ChannelLogger/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/locales/fr.po` & `limnoria-2023.4.28/plugins/ChannelLogger/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/locales/hu.po` & `limnoria-2023.4.28/plugins/ChannelLogger/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/locales/it.po` & `limnoria-2023.4.28/plugins/ChannelLogger/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/plugin.py` & `limnoria-2023.4.28/plugins/ChannelLogger/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelLogger/test.py` & `limnoria-2023.4.28/plugins/ChannelLogger/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/__init__.py` & `limnoria-2023.4.28/plugins/ChannelStats/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/config.py` & `limnoria-2023.4.28/plugins/ChannelStats/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/locales/fi.po` & `limnoria-2023.4.28/plugins/ChannelStats/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/locales/fr.po` & `limnoria-2023.4.28/plugins/ChannelStats/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/locales/it.po` & `limnoria-2023.4.28/plugins/ChannelStats/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/plugin.py` & `limnoria-2023.4.28/plugins/ChannelStats/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ChannelStats/test.py` & `limnoria-2023.4.28/plugins/ChannelStats/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/__init__.py` & `limnoria-2023.4.28/plugins/Conditional/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/config.py` & `limnoria-2023.4.28/plugins/Conditional/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/locales/fi.po` & `limnoria-2023.4.28/plugins/Conditional/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/locales/fr.po` & `limnoria-2023.4.28/plugins/Conditional/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/locales/it.po` & `limnoria-2023.4.28/plugins/Conditional/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/plugin.py` & `limnoria-2023.4.28/plugins/Conditional/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Conditional/test.py` & `limnoria-2023.4.28/plugins/Conditional/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/__init__.py` & `limnoria-2023.4.28/plugins/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/config.py` & `limnoria-2023.4.28/plugins/Config/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/locales/de.po` & `limnoria-2023.4.28/plugins/Config/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/locales/fi.po` & `limnoria-2023.4.28/plugins/Config/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/locales/fr.po` & `limnoria-2023.4.28/plugins/Config/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/locales/hu.po` & `limnoria-2023.4.28/plugins/Config/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/locales/it.po` & `limnoria-2023.4.28/plugins/Config/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/plugin.py` & `limnoria-2023.4.28/plugins/Config/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Config/test.py` & `limnoria-2023.4.28/plugins/Config/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/__init__.py` & `limnoria-2023.4.28/plugins/Ctcp/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/config.py` & `limnoria-2023.4.28/plugins/Ctcp/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/locales/de.po` & `limnoria-2023.4.28/plugins/Ctcp/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/locales/fi.po` & `limnoria-2023.4.28/plugins/Ctcp/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/locales/fr.po` & `limnoria-2023.4.28/plugins/Ctcp/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/locales/hu.po` & `limnoria-2023.4.28/plugins/Ctcp/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/locales/it.po` & `limnoria-2023.4.28/plugins/Ctcp/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/plugin.py` & `limnoria-2023.4.28/plugins/Ctcp/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Ctcp/test.py` & `limnoria-2023.4.28/plugins/Ctcp/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/DDG/__init__.py` & `limnoria-2023.4.28/plugins/DDG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/DDG/config.py` & `limnoria-2023.4.28/plugins/DDG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/DDG/parser.py` & `limnoria-2023.4.28/plugins/DDG/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/DDG/plugin.py` & `limnoria-2023.4.28/plugins/DDG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/DDG/test.py` & `limnoria-2023.4.28/plugins/DDG/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Debug/__init__.py` & `limnoria-2023.4.28/plugins/Debug/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Debug/config.py` & `limnoria-2023.4.28/plugins/Debug/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Debug/plugin.py` & `limnoria-2023.4.28/plugins/Debug/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Debug/test.py` & `limnoria-2023.4.28/plugins/Debug/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/__init__.py` & `limnoria-2023.4.28/plugins/Dict/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/config.py` & `limnoria-2023.4.28/plugins/Dict/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/local/dictclient.py` & `limnoria-2023.4.28/plugins/Dict/local/dictclient.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/locales/fi.po` & `limnoria-2023.4.28/plugins/Dict/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/locales/fr.po` & `limnoria-2023.4.28/plugins/Dict/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/locales/it.po` & `limnoria-2023.4.28/plugins/Dict/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/plugin.py` & `limnoria-2023.4.28/plugins/Dict/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dict/test.py` & `limnoria-2023.4.28/plugins/Dict/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/__init__.py` & `limnoria-2023.4.28/plugins/Dunno/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/config.py` & `limnoria-2023.4.28/plugins/Dunno/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/locales/de.po` & `limnoria-2023.4.28/plugins/Dunno/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/locales/fi.po` & `limnoria-2023.4.28/plugins/Dunno/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/locales/fr.po` & `limnoria-2023.4.28/plugins/Dunno/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/locales/it.po` & `limnoria-2023.4.28/plugins/Dunno/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/plugin.py` & `limnoria-2023.4.28/plugins/Dunno/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Dunno/test.py` & `limnoria-2023.4.28/plugins/Dunno/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/__init__.py` & `limnoria-2023.4.28/plugins/Factoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/config.py` & `limnoria-2023.4.28/plugins/Factoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/locales/fi.po` & `limnoria-2023.4.28/plugins/Factoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/locales/fr.po` & `limnoria-2023.4.28/plugins/Factoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/locales/it.po` & `limnoria-2023.4.28/plugins/Factoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/plugin.py` & `limnoria-2023.4.28/plugins/Factoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Factoids/test.py` & `limnoria-2023.4.28/plugins/Factoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/__init__.py` & `limnoria-2023.4.28/plugins/Fediverse/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/activitypub.py` & `limnoria-2023.4.28/plugins/Fediverse/activitypub.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/config.py` & `limnoria-2023.4.28/plugins/Fediverse/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/plugin.py` & `limnoria-2023.4.28/plugins/Fediverse/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/test.py` & `limnoria-2023.4.28/plugins/Fediverse/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/test_data.py` & `limnoria-2023.4.28/plugins/Fediverse/test_data.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Fediverse/utils.py` & `limnoria-2023.4.28/plugins/Fediverse/utils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/__init__.py` & `limnoria-2023.4.28/plugins/Filter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/config.py` & `limnoria-2023.4.28/plugins/Filter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/locales/fi.po` & `limnoria-2023.4.28/plugins/Filter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/locales/fr.po` & `limnoria-2023.4.28/plugins/Filter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/locales/it.po` & `limnoria-2023.4.28/plugins/Filter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/plugin.py` & `limnoria-2023.4.28/plugins/Filter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Filter/test.py` & `limnoria-2023.4.28/plugins/Filter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/__init__.py` & `limnoria-2023.4.28/plugins/Format/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/config.py` & `limnoria-2023.4.28/plugins/Format/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/locales/fi.po` & `limnoria-2023.4.28/plugins/Format/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/locales/fr.po` & `limnoria-2023.4.28/plugins/Format/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/locales/it.po` & `limnoria-2023.4.28/plugins/Format/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/plugin.py` & `limnoria-2023.4.28/plugins/Format/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Format/test.py` & `limnoria-2023.4.28/plugins/Format/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/GPG/__init__.py` & `limnoria-2023.4.28/plugins/GPG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/GPG/config.py` & `limnoria-2023.4.28/plugins/GPG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/GPG/plugin.py` & `limnoria-2023.4.28/plugins/GPG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/GPG/test.py` & `limnoria-2023.4.28/plugins/GPG/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/__init__.py` & `limnoria-2023.4.28/plugins/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/config.py` & `limnoria-2023.4.28/plugins/Games/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/locales/de.po` & `limnoria-2023.4.28/plugins/Games/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/locales/fi.po` & `limnoria-2023.4.28/plugins/Games/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/locales/fr.po` & `limnoria-2023.4.28/plugins/Games/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/locales/it.po` & `limnoria-2023.4.28/plugins/Games/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/plugin.py` & `limnoria-2023.4.28/plugins/Games/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Games/test.py` & `limnoria-2023.4.28/plugins/Games/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/__init__.py` & `limnoria-2023.4.28/plugins/Geography/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/common.py` & `limnoria-2023.4.28/plugins/Geography/common.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/config.py` & `limnoria-2023.4.28/plugins/Geography/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/nominatim.py` & `limnoria-2023.4.28/plugins/Geography/nominatim.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/plugin.py` & `limnoria-2023.4.28/plugins/Geography/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/test.py` & `limnoria-2023.4.28/plugins/Geography/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Geography/wikidata.py` & `limnoria-2023.4.28/plugins/Geography/wikidata.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/__init__.py` & `limnoria-2023.4.28/plugins/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/config.py` & `limnoria-2023.4.28/plugins/Google/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/locales/fi.po` & `limnoria-2023.4.28/plugins/Google/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/locales/fr.po` & `limnoria-2023.4.28/plugins/Google/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/locales/it.po` & `limnoria-2023.4.28/plugins/Google/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/parser.py` & `limnoria-2023.4.28/plugins/Google/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/plugin.py` & `limnoria-2023.4.28/plugins/Google/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Google/test.py` & `limnoria-2023.4.28/plugins/Google/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Hashes/__init__.py` & `limnoria-2023.4.28/plugins/Hashes/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Hashes/config.py` & `limnoria-2023.4.28/plugins/Hashes/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Hashes/plugin.py` & `limnoria-2023.4.28/plugins/Hashes/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Hashes/test.py` & `limnoria-2023.4.28/plugins/Hashes/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/__init__.py` & `limnoria-2023.4.28/plugins/Herald/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/config.py` & `limnoria-2023.4.28/plugins/Herald/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/locales/fi.po` & `limnoria-2023.4.28/plugins/Herald/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/locales/fr.po` & `limnoria-2023.4.28/plugins/Herald/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/locales/it.po` & `limnoria-2023.4.28/plugins/Herald/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/plugin.py` & `limnoria-2023.4.28/plugins/Herald/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Herald/test.py` & `limnoria-2023.4.28/plugins/Herald/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/__init__.py` & `limnoria-2023.4.28/plugins/Internet/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/config.py` & `limnoria-2023.4.28/plugins/Internet/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/locales/fi.po` & `limnoria-2023.4.28/plugins/Internet/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/locales/fr.po` & `limnoria-2023.4.28/plugins/Internet/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/locales/it.po` & `limnoria-2023.4.28/plugins/Internet/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/plugin.py` & `limnoria-2023.4.28/plugins/Internet/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Internet/test.py` & `limnoria-2023.4.28/plugins/Internet/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/__init__.py` & `limnoria-2023.4.28/plugins/Karma/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/config.py` & `limnoria-2023.4.28/plugins/Karma/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/locales/fi.po` & `limnoria-2023.4.28/plugins/Karma/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/locales/fr.po` & `limnoria-2023.4.28/plugins/Karma/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/locales/it.po` & `limnoria-2023.4.28/plugins/Karma/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/plugin.py` & `limnoria-2023.4.28/plugins/Karma/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Karma/test.py` & `limnoria-2023.4.28/plugins/Karma/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/__init__.py` & `limnoria-2023.4.28/plugins/Lart/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/config.py` & `limnoria-2023.4.28/plugins/Lart/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/locales/fi.po` & `limnoria-2023.4.28/plugins/Lart/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/locales/fr.po` & `limnoria-2023.4.28/plugins/Lart/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/locales/it.po` & `limnoria-2023.4.28/plugins/Lart/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/plugin.py` & `limnoria-2023.4.28/plugins/Lart/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Lart/test.py` & `limnoria-2023.4.28/plugins/Lart/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/__init__.py` & `limnoria-2023.4.28/plugins/Later/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/config.py` & `limnoria-2023.4.28/plugins/Later/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/locales/de.po` & `limnoria-2023.4.28/plugins/Later/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/locales/fi.po` & `limnoria-2023.4.28/plugins/Later/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/locales/fr.po` & `limnoria-2023.4.28/plugins/Later/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/locales/it.po` & `limnoria-2023.4.28/plugins/Later/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/plugin.py` & `limnoria-2023.4.28/plugins/Later/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Later/test.py` & `limnoria-2023.4.28/plugins/Later/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/__init__.py` & `limnoria-2023.4.28/plugins/Limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/config.py` & `limnoria-2023.4.28/plugins/Limiter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/locales/fi.po` & `limnoria-2023.4.28/plugins/Limiter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/locales/fr.po` & `limnoria-2023.4.28/plugins/Limiter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/locales/hu.po` & `limnoria-2023.4.28/plugins/Limiter/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/locales/it.po` & `limnoria-2023.4.28/plugins/Limiter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/plugin.py` & `limnoria-2023.4.28/plugins/Limiter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Limiter/test.py` & `limnoria-2023.4.28/plugins/Limiter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/LogToIrc/__init__.py` & `limnoria-2023.4.28/plugins/LogToIrc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/LogToIrc/config.py` & `limnoria-2023.4.28/plugins/LogToIrc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/LogToIrc/handler.py` & `limnoria-2023.4.28/plugins/LogToIrc/handler.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/LogToIrc/plugin.py` & `limnoria-2023.4.28/plugins/LogToIrc/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/LogToIrc/test.py` & `limnoria-2023.4.28/plugins/LogToIrc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/__init__.py` & `limnoria-2023.4.28/plugins/Math/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/config.py` & `limnoria-2023.4.28/plugins/Math/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/local/convertcore.py` & `limnoria-2023.4.28/plugins/Math/local/convertcore.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/locales/fi.po` & `limnoria-2023.4.28/plugins/Math/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/locales/fr.po` & `limnoria-2023.4.28/plugins/Math/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/locales/hu.po` & `limnoria-2023.4.28/plugins/Math/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/locales/it.po` & `limnoria-2023.4.28/plugins/Math/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/plugin.py` & `limnoria-2023.4.28/plugins/Math/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Math/test.py` & `limnoria-2023.4.28/plugins/Math/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/__init__.py` & `limnoria-2023.4.28/plugins/MessageParser/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/config.py` & `limnoria-2023.4.28/plugins/MessageParser/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/locales/fi.po` & `limnoria-2023.4.28/plugins/MessageParser/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/locales/fr.po` & `limnoria-2023.4.28/plugins/MessageParser/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/locales/it.po` & `limnoria-2023.4.28/plugins/MessageParser/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/plugin.py` & `limnoria-2023.4.28/plugins/MessageParser/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MessageParser/test.py` & `limnoria-2023.4.28/plugins/MessageParser/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/__init__.py` & `limnoria-2023.4.28/plugins/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/config.py` & `limnoria-2023.4.28/plugins/Misc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/locales/de.po` & `limnoria-2023.4.28/plugins/Misc/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/locales/fi.po` & `limnoria-2023.4.28/plugins/Misc/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/locales/fr.po` & `limnoria-2023.4.28/plugins/Misc/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/locales/hu.po` & `limnoria-2023.4.28/plugins/Misc/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/locales/it.po` & `limnoria-2023.4.28/plugins/Misc/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/plugin.py` & `limnoria-2023.4.28/plugins/Misc/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Misc/test.py` & `limnoria-2023.4.28/plugins/Misc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/__init__.py` & `limnoria-2023.4.28/plugins/MoobotFactoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/config.py` & `limnoria-2023.4.28/plugins/MoobotFactoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/locales/fi.po` & `limnoria-2023.4.28/plugins/MoobotFactoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/locales/fr.po` & `limnoria-2023.4.28/plugins/MoobotFactoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/locales/it.po` & `limnoria-2023.4.28/plugins/MoobotFactoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/plugin.py` & `limnoria-2023.4.28/plugins/MoobotFactoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/MoobotFactoids/test.py` & `limnoria-2023.4.28/plugins/MoobotFactoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/__init__.py` & `limnoria-2023.4.28/plugins/Network/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/config.py` & `limnoria-2023.4.28/plugins/Network/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/locales/de.po` & `limnoria-2023.4.28/plugins/Network/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/locales/fi.po` & `limnoria-2023.4.28/plugins/Network/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/locales/fr.po` & `limnoria-2023.4.28/plugins/Network/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/locales/it.po` & `limnoria-2023.4.28/plugins/Network/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/plugin.py` & `limnoria-2023.4.28/plugins/Network/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Network/test.py` & `limnoria-2023.4.28/plugins/Network/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/__init__.py` & `limnoria-2023.4.28/plugins/News/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/config.py` & `limnoria-2023.4.28/plugins/News/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/locales/fi.po` & `limnoria-2023.4.28/plugins/News/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/locales/fr.po` & `limnoria-2023.4.28/plugins/News/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/locales/it.po` & `limnoria-2023.4.28/plugins/News/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/plugin.py` & `limnoria-2023.4.28/plugins/News/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/News/test.py` & `limnoria-2023.4.28/plugins/News/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/__init__.py` & `limnoria-2023.4.28/plugins/NickAuth/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/config.py` & `limnoria-2023.4.28/plugins/NickAuth/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/locales/de.po` & `limnoria-2023.4.28/plugins/NickAuth/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/locales/fi.po` & `limnoria-2023.4.28/plugins/NickAuth/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/plugin.py` & `limnoria-2023.4.28/plugins/NickAuth/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickAuth/test.py` & `limnoria-2023.4.28/plugins/NickAuth/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/__init__.py` & `limnoria-2023.4.28/plugins/NickCapture/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/config.py` & `limnoria-2023.4.28/plugins/NickCapture/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/locales/de.po` & `limnoria-2023.4.28/plugins/NickCapture/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/locales/fi.po` & `limnoria-2023.4.28/plugins/NickCapture/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/locales/fr.po` & `limnoria-2023.4.28/plugins/NickCapture/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/locales/it.po` & `limnoria-2023.4.28/plugins/NickCapture/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/plugin.py` & `limnoria-2023.4.28/plugins/NickCapture/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/NickCapture/test.py` & `limnoria-2023.4.28/plugins/NickCapture/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/__init__.py` & `limnoria-2023.4.28/plugins/Nickometer/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/config.py` & `limnoria-2023.4.28/plugins/Nickometer/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/locales/fi.po` & `limnoria-2023.4.28/plugins/Nickometer/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/locales/fr.po` & `limnoria-2023.4.28/plugins/Nickometer/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/locales/it.po` & `limnoria-2023.4.28/plugins/Nickometer/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/plugin.py` & `limnoria-2023.4.28/plugins/Nickometer/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Nickometer/test.py` & `limnoria-2023.4.28/plugins/Nickometer/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/__init__.py` & `limnoria-2023.4.28/plugins/Note/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/config.py` & `limnoria-2023.4.28/plugins/Note/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/locales/fi.po` & `limnoria-2023.4.28/plugins/Note/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/locales/fr.po` & `limnoria-2023.4.28/plugins/Note/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/locales/it.po` & `limnoria-2023.4.28/plugins/Note/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/plugin.py` & `limnoria-2023.4.28/plugins/Note/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Note/test.py` & `limnoria-2023.4.28/plugins/Note/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/__init__.py` & `limnoria-2023.4.28/plugins/Owner/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/config.py` & `limnoria-2023.4.28/plugins/Owner/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/locales/de.po` & `limnoria-2023.4.28/plugins/Owner/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/locales/fi.po` & `limnoria-2023.4.28/plugins/Owner/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/locales/fr.po` & `limnoria-2023.4.28/plugins/Owner/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/locales/hu.po` & `limnoria-2023.4.28/plugins/Owner/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/locales/it.po` & `limnoria-2023.4.28/plugins/Owner/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/plugin.py` & `limnoria-2023.4.28/plugins/Owner/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Owner/test.py` & `limnoria-2023.4.28/plugins/Owner/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/__init__.py` & `limnoria-2023.4.28/plugins/Plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/config.py` & `limnoria-2023.4.28/plugins/Plugin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/locales/de.po` & `limnoria-2023.4.28/plugins/Plugin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/locales/fi.po` & `limnoria-2023.4.28/plugins/Plugin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/locales/fr.po` & `limnoria-2023.4.28/plugins/Plugin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/locales/it.po` & `limnoria-2023.4.28/plugins/Plugin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/plugin.py` & `limnoria-2023.4.28/plugins/Plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Plugin/test.py` & `limnoria-2023.4.28/plugins/Plugin/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/__init__.py` & `limnoria-2023.4.28/plugins/PluginDownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/config.py` & `limnoria-2023.4.28/plugins/PluginDownloader/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/locales/de.po` & `limnoria-2023.4.28/plugins/PluginDownloader/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/locales/fi.po` & `limnoria-2023.4.28/plugins/PluginDownloader/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/locales/fr.po` & `limnoria-2023.4.28/plugins/PluginDownloader/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/locales/it.po` & `limnoria-2023.4.28/plugins/PluginDownloader/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/plugin.py` & `limnoria-2023.4.28/plugins/PluginDownloader/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/PluginDownloader/test.py` & `limnoria-2023.4.28/plugins/PluginDownloader/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Poll/__init__.py` & `limnoria-2023.4.28/plugins/Poll/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Poll/config.py` & `limnoria-2023.4.28/plugins/Poll/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Poll/plugin.py` & `limnoria-2023.4.28/plugins/Poll/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Poll/test.py` & `limnoria-2023.4.28/plugins/Poll/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/__init__.py` & `limnoria-2023.4.28/plugins/Praise/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/config.py` & `limnoria-2023.4.28/plugins/Praise/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/locales/fi.po` & `limnoria-2023.4.28/plugins/Praise/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/locales/fr.po` & `limnoria-2023.4.28/plugins/Praise/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/locales/it.po` & `limnoria-2023.4.28/plugins/Praise/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/plugin.py` & `limnoria-2023.4.28/plugins/Praise/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Praise/test.py` & `limnoria-2023.4.28/plugins/Praise/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/__init__.py` & `limnoria-2023.4.28/plugins/Protector/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/config.py` & `limnoria-2023.4.28/plugins/Protector/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/locales/fi.po` & `limnoria-2023.4.28/plugins/Protector/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/locales/fr.po` & `limnoria-2023.4.28/plugins/Protector/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/locales/it.po` & `limnoria-2023.4.28/plugins/Protector/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/plugin.py` & `limnoria-2023.4.28/plugins/Protector/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Protector/test.py` & `limnoria-2023.4.28/plugins/Protector/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/__init__.py` & `limnoria-2023.4.28/plugins/Quote/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/config.py` & `limnoria-2023.4.28/plugins/Quote/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/locales/fi.po` & `limnoria-2023.4.28/plugins/Quote/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/locales/fr.po` & `limnoria-2023.4.28/plugins/Quote/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/locales/it.po` & `limnoria-2023.4.28/plugins/Quote/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/plugin.py` & `limnoria-2023.4.28/plugins/Quote/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Quote/test.py` & `limnoria-2023.4.28/plugins/Quote/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/__init__.py` & `limnoria-2023.4.28/plugins/QuoteGrabs/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/config.py` & `limnoria-2023.4.28/plugins/QuoteGrabs/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/locales/fi.po` & `limnoria-2023.4.28/plugins/QuoteGrabs/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/locales/fr.po` & `limnoria-2023.4.28/plugins/QuoteGrabs/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/locales/it.po` & `limnoria-2023.4.28/plugins/QuoteGrabs/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/plugin.py` & `limnoria-2023.4.28/plugins/QuoteGrabs/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/QuoteGrabs/test.py` & `limnoria-2023.4.28/plugins/QuoteGrabs/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/__init__.py` & `limnoria-2023.4.28/plugins/RSS/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/config.py` & `limnoria-2023.4.28/plugins/RSS/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/locales/de.po` & `limnoria-2023.4.28/plugins/RSS/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/locales/fi.po` & `limnoria-2023.4.28/plugins/RSS/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/locales/fr.po` & `limnoria-2023.4.28/plugins/RSS/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/locales/hu.po` & `limnoria-2023.4.28/plugins/RSS/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/locales/it.po` & `limnoria-2023.4.28/plugins/RSS/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/plugin.py` & `limnoria-2023.4.28/plugins/RSS/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/RSS/test.py` & `limnoria-2023.4.28/plugins/RSS/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/__init__.py` & `limnoria-2023.4.28/plugins/Relay/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/config.py` & `limnoria-2023.4.28/plugins/Relay/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/locales/fi.po` & `limnoria-2023.4.28/plugins/Relay/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/locales/fr.po` & `limnoria-2023.4.28/plugins/Relay/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/locales/it.po` & `limnoria-2023.4.28/plugins/Relay/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/plugin.py` & `limnoria-2023.4.28/plugins/Relay/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Relay/test.py` & `limnoria-2023.4.28/plugins/Relay/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/__init__.py` & `limnoria-2023.4.28/plugins/Reply/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/config.py` & `limnoria-2023.4.28/plugins/Reply/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/locales/de.po` & `limnoria-2023.4.28/plugins/Reply/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/locales/fi.po` & `limnoria-2023.4.28/plugins/Reply/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/locales/fr.po` & `limnoria-2023.4.28/plugins/Reply/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/locales/hu.po` & `limnoria-2023.4.28/plugins/Reply/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/locales/it.po` & `limnoria-2023.4.28/plugins/Reply/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/plugin.py` & `limnoria-2023.4.28/plugins/Reply/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Reply/test.py` & `limnoria-2023.4.28/plugins/Reply/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/__init__.py` & `limnoria-2023.4.28/plugins/Scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/config.py` & `limnoria-2023.4.28/plugins/Scheduler/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/locales/fi.po` & `limnoria-2023.4.28/plugins/Scheduler/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/locales/fr.po` & `limnoria-2023.4.28/plugins/Scheduler/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/locales/it.po` & `limnoria-2023.4.28/plugins/Scheduler/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/plugin.py` & `limnoria-2023.4.28/plugins/Scheduler/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Scheduler/test.py` & `limnoria-2023.4.28/plugins/Scheduler/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/SedRegex/__init__.py` & `limnoria-2023.4.28/plugins/SedRegex/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/SedRegex/config.py` & `limnoria-2023.4.28/plugins/SedRegex/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/SedRegex/constants.py` & `limnoria-2023.4.28/plugins/SedRegex/constants.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/SedRegex/plugin.py` & `limnoria-2023.4.28/plugins/SedRegex/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/SedRegex/test.py` & `limnoria-2023.4.28/plugins/SedRegex/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/__init__.py` & `limnoria-2023.4.28/plugins/Seen/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/config.py` & `limnoria-2023.4.28/plugins/Seen/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/locales/de.po` & `limnoria-2023.4.28/plugins/Seen/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/locales/fi.po` & `limnoria-2023.4.28/plugins/Seen/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/locales/fr.po` & `limnoria-2023.4.28/plugins/Seen/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/locales/it.po` & `limnoria-2023.4.28/plugins/Seen/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/plugin.py` & `limnoria-2023.4.28/plugins/Seen/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Seen/test.py` & `limnoria-2023.4.28/plugins/Seen/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/__init__.py` & `limnoria-2023.4.28/plugins/Services/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/config.py` & `limnoria-2023.4.28/plugins/Services/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/locales/de.po` & `limnoria-2023.4.28/plugins/Services/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/locales/fi.po` & `limnoria-2023.4.28/plugins/Services/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/locales/fr.po` & `limnoria-2023.4.28/plugins/Services/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/locales/it.po` & `limnoria-2023.4.28/plugins/Services/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/plugin.py` & `limnoria-2023.4.28/plugins/Services/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Services/test.py` & `limnoria-2023.4.28/plugins/Services/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/__init__.py` & `limnoria-2023.4.28/plugins/ShrinkUrl/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/config.py` & `limnoria-2023.4.28/plugins/ShrinkUrl/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/locales/fi.po` & `limnoria-2023.4.28/plugins/ShrinkUrl/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/locales/fr.po` & `limnoria-2023.4.28/plugins/ShrinkUrl/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/locales/it.po` & `limnoria-2023.4.28/plugins/ShrinkUrl/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/plugin.py` & `limnoria-2023.4.28/plugins/ShrinkUrl/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/ShrinkUrl/test.py` & `limnoria-2023.4.28/plugins/ShrinkUrl/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/__init__.py` & `limnoria-2023.4.28/plugins/Status/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/config.py` & `limnoria-2023.4.28/plugins/Status/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/locales/de.po` & `limnoria-2023.4.28/plugins/Status/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/locales/fi.po` & `limnoria-2023.4.28/plugins/Status/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/locales/fr.po` & `limnoria-2023.4.28/plugins/Status/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/locales/it.po` & `limnoria-2023.4.28/plugins/Status/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/plugin.py` & `limnoria-2023.4.28/plugins/Status/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Status/test.py` & `limnoria-2023.4.28/plugins/Status/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/__init__.py` & `limnoria-2023.4.28/plugins/String/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/config.py` & `limnoria-2023.4.28/plugins/String/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/locales/fi.po` & `limnoria-2023.4.28/plugins/String/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/locales/fr.po` & `limnoria-2023.4.28/plugins/String/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/locales/it.po` & `limnoria-2023.4.28/plugins/String/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/plugin.py` & `limnoria-2023.4.28/plugins/String/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/String/test.py` & `limnoria-2023.4.28/plugins/String/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/__init__.py` & `limnoria-2023.4.28/plugins/Success/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/config.py` & `limnoria-2023.4.28/plugins/Success/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/locales/fi.po` & `limnoria-2023.4.28/plugins/Success/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/locales/fr.po` & `limnoria-2023.4.28/plugins/Success/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/locales/it.po` & `limnoria-2023.4.28/plugins/Success/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/plugin.py` & `limnoria-2023.4.28/plugins/Success/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Success/test.py` & `limnoria-2023.4.28/plugins/Success/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/__init__.py` & `limnoria-2023.4.28/plugins/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/config.py` & `limnoria-2023.4.28/plugins/Time/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/locales/de.po` & `limnoria-2023.4.28/plugins/Time/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/locales/fi.po` & `limnoria-2023.4.28/plugins/Time/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/locales/fr.po` & `limnoria-2023.4.28/plugins/Time/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/locales/hu.po` & `limnoria-2023.4.28/plugins/Time/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/locales/it.po` & `limnoria-2023.4.28/plugins/Time/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/plugin.py` & `limnoria-2023.4.28/plugins/Time/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Time/test.py` & `limnoria-2023.4.28/plugins/Time/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/__init__.py` & `limnoria-2023.4.28/plugins/Todo/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/config.py` & `limnoria-2023.4.28/plugins/Todo/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/locales/de.po` & `limnoria-2023.4.28/plugins/Todo/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/locales/fi.po` & `limnoria-2023.4.28/plugins/Todo/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/locales/fr.po` & `limnoria-2023.4.28/plugins/Todo/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/locales/it.po` & `limnoria-2023.4.28/plugins/Todo/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/plugin.py` & `limnoria-2023.4.28/plugins/Todo/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Todo/test.py` & `limnoria-2023.4.28/plugins/Todo/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/__init__.py` & `limnoria-2023.4.28/plugins/Topic/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/config.py` & `limnoria-2023.4.28/plugins/Topic/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/locales/fi.po` & `limnoria-2023.4.28/plugins/Topic/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/locales/fr.po` & `limnoria-2023.4.28/plugins/Topic/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/locales/it.po` & `limnoria-2023.4.28/plugins/Topic/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/plugin.py` & `limnoria-2023.4.28/plugins/Topic/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Topic/test.py` & `limnoria-2023.4.28/plugins/Topic/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/__init__.py` & `limnoria-2023.4.28/plugins/URL/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/config.py` & `limnoria-2023.4.28/plugins/URL/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/locales/fi.po` & `limnoria-2023.4.28/plugins/URL/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/locales/fr.po` & `limnoria-2023.4.28/plugins/URL/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/locales/it.po` & `limnoria-2023.4.28/plugins/URL/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/plugin.py` & `limnoria-2023.4.28/plugins/URL/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/URL/test.py` & `limnoria-2023.4.28/plugins/URL/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/__init__.py` & `limnoria-2023.4.28/plugins/Unix/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/config.py` & `limnoria-2023.4.28/plugins/Unix/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/locales/fi.po` & `limnoria-2023.4.28/plugins/Unix/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/locales/fr.po` & `limnoria-2023.4.28/plugins/Unix/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/locales/it.po` & `limnoria-2023.4.28/plugins/Unix/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/plugin.py` & `limnoria-2023.4.28/plugins/Unix/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Unix/test.py` & `limnoria-2023.4.28/plugins/Unix/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/__init__.py` & `limnoria-2023.4.28/plugins/User/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/config.py` & `limnoria-2023.4.28/plugins/User/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/locales/de.po` & `limnoria-2023.4.28/plugins/User/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/locales/fi.po` & `limnoria-2023.4.28/plugins/User/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/locales/fr.po` & `limnoria-2023.4.28/plugins/User/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/locales/hu.po` & `limnoria-2023.4.28/plugins/User/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/locales/it.po` & `limnoria-2023.4.28/plugins/User/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/plugin.py` & `limnoria-2023.4.28/plugins/User/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/User/test.py` & `limnoria-2023.4.28/plugins/User/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/__init__.py` & `limnoria-2023.4.28/plugins/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/config.py` & `limnoria-2023.4.28/plugins/Utilities/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/locales/de.po` & `limnoria-2023.4.28/plugins/Utilities/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/locales/fi.po` & `limnoria-2023.4.28/plugins/Utilities/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/locales/fr.po` & `limnoria-2023.4.28/plugins/Utilities/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/locales/it.po` & `limnoria-2023.4.28/plugins/Utilities/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/plugin.py` & `limnoria-2023.4.28/plugins/Utilities/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Utilities/test.py` & `limnoria-2023.4.28/plugins/Utilities/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/__init__.py` & `limnoria-2023.4.28/plugins/Web/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/config.py` & `limnoria-2023.4.28/plugins/Web/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/locales/de.po` & `limnoria-2023.4.28/plugins/Web/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/locales/fi.po` & `limnoria-2023.4.28/plugins/Web/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/locales/fr.po` & `limnoria-2023.4.28/plugins/Web/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/locales/it.po` & `limnoria-2023.4.28/plugins/Web/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/plugin.py` & `limnoria-2023.4.28/plugins/Web/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/Web/test.py` & `limnoria-2023.4.28/plugins/Web/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/plugins/__init__.py` & `limnoria-2023.4.28/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/requirements.txt` & `limnoria-2023.4.28/requirements.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/scripts/supybot` & `limnoria-2023.4.28/src/scripts/limnoria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-
 ###
 # Copyright (c) 2003-2004, Jeremiah Fincher
 # Copyright (c) 2009, James McCoy
 # Copyright (c) 2010-2021, Valentin Lorentz
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -31,16 +29,14 @@
 # POSSIBILITY OF SUCH DAMAGE.
 ###
 
 """
 This is the main program to run Supybot.
 """
 
-import supybot
-
 import re
 import os
 import sys
 import atexit
 import shutil
 import signal
 
@@ -74,19 +70,22 @@
     For your information, Supybot's libraries are installed here:
     %s\n""" %
     (sys.executable, '\n    '.join(supybot.__path__)))
     exit(-1)
 
 from supybot.version import version
 
-def main():
+def run():
+    import supybot.log as log
     import supybot.conf as conf
     import supybot.world as world
     import supybot.drivers as drivers
+    import supybot.ircmsgs as ircmsgs
     import supybot.schedule as schedule
+    import supybot.httpserver as httpserver
     # We schedule this event rather than have it actually run because if there
     # is a failure between now and the time it takes the Owner plugin to load
     # all the various plugins, our registry file might be wiped.  That's bad.
     interrupted = False
     when = conf.supybot.upkeepInterval()
     schedule.addPeriodicEvent(world.upkeep, when, name='upkeep', now=False)
     world.startedAt = started
@@ -143,15 +142,15 @@
     now = time.time()
     seconds = now - world.startedAt
     log.info('Total uptime: %s.', utils.gen.timeElapsed(seconds))
     (user, system, _, _, _) = os.times()
     log.info('Total CPU time taken: %.2f seconds.', user+system)
     log.info('No more Irc objects, exiting.')
 
-if __name__ == '__main__':
+def main():
     parser = optparse.OptionParser(usage='Usage: %prog [options] configFile',
                                    version='Limnoria %s running on Python %s' %
                                    (version, sys.version))
     parser.add_option('-P', '--profile', action='store_true', dest='profile',
                       help='enables profiling')
     parser.add_option('-n', '--nick', action='store',
                       dest='nick', default='',
@@ -351,22 +350,22 @@
 
     import supybot.irclib as irclib
     import supybot.ircmsgs as ircmsgs
     import supybot.drivers as drivers
     import supybot.callbacks as callbacks
     import supybot.plugins.Owner as Owner
 
-    # These may take some resources, and it does not need to be run while boot, so
+    # This may take some resources, and it does not need to run while booting, so
     # we import it as late as possible (but before plugins are loaded).
     import supybot.httpserver as httpserver
 
     owner = Owner.Class()
 
     if options.profile:
         import profile
         world.profiling = True
-        profile.run('main()', '%s-%i.prof' % (nick, time.time()))
+        profile.run('run()', '%s-%i.prof' % (nick, time.time()))
     else:
-        main()
+        run()
 
 
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-adduser` & `limnoria-2023.4.28/src/scripts/limnoria_adduser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/scripts/supybot-botchk` & `limnoria-2023.4.28/src/scripts/limnoria_botchk.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 def debug(s):
     if VERBOSE:
         if not s.endswith(os.linesep):
             s += os.linesep
         sys.stdout.write(s)
 
-if __name__ == '__main__':
+def main():
     # XXX I wanted this for conf.version, but this will create directories. We
     # really need to refactor conf so it either doesn't create directories, or
     # so that static information (like the version) can be imported from
     # somewhere else.
     # import supybot.conf as conf
     import os
     import sys
@@ -131,8 +131,11 @@
         ret = inst.wait()
         debug('Bot started, command line %r returned %s.' % (' '.join(cmdline),
                                                              ret))
         sys.exit(ret)
     else:
         sys.exit(0)
 
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-plugin-create` & `limnoria-2023.4.28/src/scripts/limnoria_plugin_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 # vim:set shiftwidth=4 tabstop=4 expandtab textwidth=79:
 '''.lstrip()
 
 readmeTemplate = '''
 %s
 '''.lstrip()
 
-def main():
+def _main():
     global copyright
     global license
     parser = optparse.OptionParser(usage='Usage: %prog [options]',
                                    version='Supybot %s' % conf.version)
     parser.add_option('-n', '--name', action='store', dest='name',
                       help='sets the name for the plugin.')
     parser.add_option('-t', '--thread', action='store_true', dest='threaded',
@@ -303,17 +303,20 @@
     pathname = os.path.join(pathname, 'local')
     os.mkdir(pathname)
     writeFile('__init__.py',
               '# Stub so local is a module, used for third-party modules\n')
 
     print('Your new plugin template is in the %s directory.' % name)
 
-if __name__ == '__main__':
+def main():
     try:
-        main()
+        _main()
     except KeyboardInterrupt:
         print()
         output("""It looks like you cancelled out of this script before it was
         finished.  Obviously, nothing was written, but just run this script
         again whenever you want to generate a template for a plugin.""")
 
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-plugin-doc` & `limnoria-2023.4.28/src/scripts/limnoria_plugin_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         fd.close()
         error('Unknown render format: `%s\'' % options.format)
     try:
         fd.write(f())
     finally:
         fd.close()
 
-if __name__ == '__main__':
+def main():
     import glob
     import os.path
     import optparse
     import supybot.plugin as plugin
 
     parser = optparse.OptionParser(usage='Usage: %prog [options] [plugins]',
                                    version='Supybot %s' % conf.version)
@@ -345,8 +345,12 @@
         # (such as "Shutdown initiated." and friends, from atexit callbacks)
         # would result in errors.
         log._handler.setLevel(logging.CRITICAL)
         shutil.rmtree(conf.supybot.directories.log())
         shutil.rmtree(conf.supybot.directories.conf())
         shutil.rmtree(conf.supybot.directories.data())
 
+
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=78:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-reset-password` & `limnoria-2023.4.28/src/scripts/limnoria_reset_password.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 from supybot.questions import *
 
 import os
 import sys
 import optparse
 
-def main():
+def _main():
     import supybot.log as log
     import supybot.conf as conf
     conf.supybot.log.stdout.setValue(False)
     parser = optparse.OptionParser(usage='Usage: %prog [options] <users.conf>',
                                    version='supybot %s' % conf.version)
     parser.add_option('-u', '--username', action='store', default='',
                       dest='name',
@@ -98,14 +98,17 @@
     user = ircdb.users.getUser(name)
     user.setPassword(password)
     ircdb.users.setUser(user)
     ircdb.users.flush()
     ircdb.users.close()
     print('User %s\'s password reset!' % name)
 
-if __name__ == '__main__':
+def main():
     try:
         main()
     except KeyboardInterrupt:
         pass
 
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-test` & `limnoria-2023.4.28/src/scripts/limnoria_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     """A class to represent platform-independent paths."""
     _r = re.compile(r'[\\/]')
     def __hash__(self):
         return reduce(lambda h, s: h ^ hash(s), self._r.split(self), 0)
     def __eq__(self, other):
         return self._r.split(self) == self._r.split(other)
 
-if __name__ == '__main__':
+def main():
     import glob
     import os.path
     import optparse
     import supybot.test as test
     import supybot.plugin as plugin
 
     parser = optparse.OptionParser(usage='Usage: %prog [options] [plugins]',
@@ -239,8 +239,12 @@
         print('Total asserts: %s' % unittest.asserts)
 
     if result.wasSuccessful():
         sys.exit(0)
     else:
         sys.exit(1)
 
+
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/scripts/supybot-wizard` & `limnoria-2023.4.28/src/scripts/limnoria_wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 output("""Sorry, I couldn't make that directory for some
                 reason.  The Operating System told me %s.  You're going to
                 have to pick someplace else.""" % e)
                 prompt = True
     return (dir, os.path.dirname(orig_dir))
 
 
-def main():
+def _main():
     import supybot.version as version
     parser = optparse.OptionParser(usage='Usage: %prog [options]',
                                    version='Supybot %s' % version.version)
     parser.add_option('', '--allow-root', action='store_true',
                       dest='allowRoot',
                       help='Determines whether the wizard will be allowed to '
                            'as root. This should not be used except in special '
@@ -811,22 +811,26 @@
     # Done!
     output("""All done!  Your new bot configuration is %s.  If you're running
     a *nix based OS, you can probably start your bot with the command line
     "supybot %s".  If you're not running a *nix or similar machine, you'll
     just have to start it like you start all your other Python scripts.""" % \
                                                          (filename, filename))
 
-if __name__ == '__main__':
+def main():
     try:
-        main()
+        _main()
     except KeyboardInterrupt:
         # We may still be using bold text when exiting during a prompt
         if questions.useBold:
             import supybot.ansi as ansi
             print(ansi.RESET)
         print()
         print()
         output("""Well, it looks like you canceled out of the wizard before
         it was done.  Unfortunately, I didn't get to write anything to file.
         Please run the wizard again to completion.""")
 
+
+if __name__ == '__main__':
+    main()
+
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/setup.py` & `limnoria-2023.4.28/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,15 +113,17 @@
 plugins = [s for s in os.listdir('plugins') if
            os.path.exists(os.path.join('plugins', s, 'plugin.py'))]
 
 packages = ['supybot',
             'supybot.locales',
             'supybot.utils',
             'supybot.drivers',
-            'supybot.plugins',] + \
+            'supybot.plugins',
+            'supybot.scripts',
+            ] + \
             ['supybot.plugins.'+s for s in plugins] + \
             [
              'supybot.plugins.Dict.local',
              'supybot.plugins.Math.local',
             ]
 
 package_dir = {'supybot': 'src',
@@ -148,14 +150,25 @@
 
     if os.path.exists(locales_path):
         files.extend(['locales/'+s for s in os.listdir(locales_path)])
 
     if files:
         package_data.update({plugin_name: files})
 
+scripts = [
+    '',
+    '-test',
+    '-botchk',
+    '-wizard',
+    '-adduser',
+    '-reset-password',
+    '-plugin-doc',
+    '-plugin-create',
+]
+
 setup(
     # Metadata
     name='limnoria',
     provides=['supybot'],
     version=version,
     author='Valentin Lorentz',
     url='https://limnoria.net/',
@@ -198,29 +211,26 @@
     # Installation data
     packages=packages,
 
     package_dir=package_dir,
 
     package_data=package_data,
 
-    scripts=['scripts/supybot',
-             'scripts/supybot-test',
-             'scripts/supybot-botchk',
-             'scripts/supybot-wizard',
-             'scripts/supybot-adduser',
-             'scripts/supybot-reset-password',
-             'scripts/supybot-plugin-doc',
-             'scripts/supybot-plugin-create',
-             ],
-    data_files=[('share/man/man1', ['man/supybot.1']),
-                ('share/man/man1', ['man/supybot-test.1']),
-                ('share/man/man1', ['man/supybot-botchk.1']),
-                ('share/man/man1', ['man/supybot-wizard.1']),
-                ('share/man/man1', ['man/supybot-adduser.1']),
-                ('share/man/man1', ['man/supybot-reset-password.1']),
-                ('share/man/man1', ['man/supybot-plugin-doc.1']),
-                ('share/man/man1', ['man/supybot-plugin-create.1']),
-        ],
-
-    )
+    entry_points={
+        'console_scripts': [
+            '%s%s = supybot.scripts.limnoria%s:main'
+            % (prefix, name, name.replace('-', '_'))
+            for name in scripts
+            for prefix in ('supybot', 'limnoria')
+        ]
+    },
+
+    data_files=[
+        ('share/man/man1', [
+            'man/%s%s.1' % (prefix, name)
+            for name in scripts
+            for prefix in ('supybot', 'limnoria')
+        ]),
+    ],
+)
 
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.1.28/src/__init__.py` & `limnoria-2023.4.28/src/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/ansi.py` & `limnoria-2023.4.28/src/ansi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/callbacks.py` & `limnoria-2023.4.28/src/callbacks.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/cdb.py` & `limnoria-2023.4.28/src/cdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/commands.py` & `limnoria-2023.4.28/src/commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/conf.py` & `limnoria-2023.4.28/src/conf.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/dbi.py` & `limnoria-2023.4.28/src/dbi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/drivers/Socket.py` & `limnoria-2023.4.28/src/drivers/Socket.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,14 @@
         self.irc = irc
         drivers.IrcDriver.__init__(self, irc)
         drivers.ServersMixin.__init__(self, irc)
         self.conn = None
         self._attempt = -1
         self.servers = ()
         self.eagains = 0
-        self.inbuffer = b''
-        self.outbuffer = ''
         self.zombie = False
         self.connected = False
         self.writeCheckTime = None
         self.nextReconnectTime = None
         self.resetDelay()
         if self.networkGroup.get('ssl')() and 'ssl' not in globals():
             drivers.log.error('The Socket driver can not connect to SSL '
@@ -244,14 +242,16 @@
             self._sendIfMsgs()
 
     def connect(self, **kwargs):
         self.reconnect(reset=False, **kwargs)
 
     def reconnect(self, wait=False, reset=True, server=None):
         self._attempt += 1
+        self.inbuffer = b''
+        self.outbuffer = ''
         self.nextReconnectTime = None
         if self.connected:
             self.onDisconnect()
             drivers.log.reconnect(self.irc.network)
             if self in self._instances:
                 self._instances.remove(self)
             try:
```

### Comparing `limnoria-2023.1.28/src/drivers/__init__.py` & `limnoria-2023.4.28/src/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/dynamicScope.py` & `limnoria-2023.4.28/src/dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/gpg.py` & `limnoria-2023.4.28/src/gpg.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/httpserver.py` & `limnoria-2023.4.28/src/httpserver.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/i18n.py` & `limnoria-2023.4.28/src/i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/ircdb.py` & `limnoria-2023.4.28/src/ircdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/irclib.py` & `limnoria-2023.4.28/src/irclib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1772,15 +1772,16 @@
 
 
     # Note: echo-message is only requested if labeled-response is available.
     REQUEST_CAPABILITIES = set(['account-notify', 'extended-join',
         'multi-prefix', 'metadata-notify', 'account-tag',
         'userhost-in-names', 'invite-notify', 'server-time',
         'chghost', 'batch', 'away-notify', 'message-tags',
-        'msgid', 'setname', 'labeled-response', 'echo-message'])
+        'msgid', 'setname', 'labeled-response', 'echo-message',
+        'standard-replies'])
     """IRCv3 capabilities requested when they are available.
 
     echo-message is special-cased to be requested only with labeled-response.
 
     To check if a capability was negotiated, use `irc.state.capabilities_ack`.
     """
```

### Comparing `limnoria-2023.1.28/src/ircmsgs.py` & `limnoria-2023.4.28/src/ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/ircutils.py` & `limnoria-2023.4.28/src/ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/log.py` & `limnoria-2023.4.28/src/log.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/plugin.py` & `limnoria-2023.4.28/src/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/questions.py` & `limnoria-2023.4.28/src/questions.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/registry.py` & `limnoria-2023.4.28/src/registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/schedule.py` & `limnoria-2023.4.28/src/schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/setup.py` & `limnoria-2023.4.28/src/setup.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/shlex.py` & `limnoria-2023.4.28/src/shlex.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/test.py` & `limnoria-2023.4.28/src/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/unpreserve.py` & `limnoria-2023.4.28/src/unpreserve.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/__init__.py` & `limnoria-2023.4.28/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/crypt.py` & `limnoria-2023.4.28/src/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/error.py` & `limnoria-2023.4.28/src/utils/error.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/file.py` & `limnoria-2023.4.28/src/utils/file.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/gen.py` & `limnoria-2023.4.28/src/utils/gen.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/iter.py` & `limnoria-2023.4.28/src/utils/iter.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/math_evaluator.py` & `limnoria-2023.4.28/src/utils/math_evaluator.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/minisix.py` & `limnoria-2023.4.28/src/utils/minisix.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/net.py` & `limnoria-2023.4.28/src/utils/net.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/python.py` & `limnoria-2023.4.28/src/utils/python.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/seq.py` & `limnoria-2023.4.28/src/utils/seq.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/str.py` & `limnoria-2023.4.28/src/utils/str.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/structures.py` & `limnoria-2023.4.28/src/utils/structures.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/time.py` & `limnoria-2023.4.28/src/utils/time.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/transaction.py` & `limnoria-2023.4.28/src/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/utils/web.py` & `limnoria-2023.4.28/src/utils/web.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/src/world.py` & `limnoria-2023.4.28/src/world.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/__init__.py` & `limnoria-2023.4.28/test/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test.py` & `limnoria-2023.4.28/test/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_callbacks.py` & `limnoria-2023.4.28/test/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_commands.py` & `limnoria-2023.4.28/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_conf.py` & `limnoria-2023.4.28/test/test_conf.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_drivers.py` & `limnoria-2023.4.28/test/test_drivers.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_dynamicScope.py` & `limnoria-2023.4.28/test/test_dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_firewall.py` & `limnoria-2023.4.28/test/test_firewall.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_format.py` & `limnoria-2023.4.28/test/test_format.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_i18n.py` & `limnoria-2023.4.28/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_ircdb.py` & `limnoria-2023.4.28/test/test_ircdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_irclib.py` & `limnoria-2023.4.28/test/test_irclib.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_ircmsgs.py` & `limnoria-2023.4.28/test/test_ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_ircutils.py` & `limnoria-2023.4.28/test/test_ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_misc.py` & `limnoria-2023.4.28/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_plugin.py` & `limnoria-2023.4.28/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_plugin_create.py` & `limnoria-2023.4.28/test/test_plugin_create.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_plugins.py` & `limnoria-2023.4.28/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_registry.py` & `limnoria-2023.4.28/test/test_registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_schedule.py` & `limnoria-2023.4.28/test/test_schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_standardSubstitute.py` & `limnoria-2023.4.28/test/test_standardSubstitute.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_utils.py` & `limnoria-2023.4.28/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.1.28/test/test_yn.py` & `limnoria-2023.4.28/test/test_yn.py`

 * *Files identical despite different names*

