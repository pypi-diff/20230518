# Comparing `tmp/multidecoder-0.0.8.tar.gz` & `tmp/multidecoder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidecoder-0.0.8.tar", last modified: Thu Apr 28 15:57:21 2022, max compression
+gzip compressed data, was "multidecoder-0.0.9.tar", last modified: Tue May  3 17:13:01 2022, max compression
```

## Comparing `multidecoder-0.0.8.tar` & `multidecoder-0.0.9.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.448037 multidecoder-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-04-28 15:56:20.000000 multidecoder-0.0.8/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-04-28 15:56:20.000000 multidecoder-0.0.8/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-04-28 15:57:21.448037 multidecoder-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1657 2022-04-28 15:56:20.000000 multidecoder-0.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.432037 multidecoder-0.0.8/multidecoder/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      142 2022-04-28 15:57:20.000000 multidecoder-0.0.8/multidecoder/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.436037 multidecoder-0.0.8/multidecoder/analyzers/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1822 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/base64.py
--rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/concat.py
--rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/encoding.py
--rw-r--r--   0 vsts      (1001) docker     (121)      444 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/filename.py
--rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/hex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3930 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/network.py
--rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/path.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3706 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/shell.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1108 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/vba.py
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/analyzers/xml.py
--rw-r--r--   0 vsts      (1001) docker     (121)    22373 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/domains.py
--rw-r--r--   0 vsts      (1001) docker     (121)      808 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/hit.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1987 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/json_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1067 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keyword.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.436037 multidecoder-0.0.8/multidecoder/keywords/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.444037 multidecoder-0.0.8/multidecoder/keywords/api/
--rw-r--r--   0 vsts      (1001) docker     (121)     4040 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.advapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       23 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.apphelp
--rw-r--r--   0 vsts      (1001) docker     (121)     1212 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.atl
--rw-r--r--   0 vsts      (1001) docker     (121)      243 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.atl80
--rw-r--r--   0 vsts      (1001) docker     (121)      229 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.atl90
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.au3zip
--rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.avicap32
--rw-r--r--   0 vsts      (1001) docker     (121)      196 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.cabinet
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.clbcatq
--rw-r--r--   0 vsts      (1001) docker     (121)       56 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.cmdial32
--rw-r--r--   0 vsts      (1001) docker     (121)      177 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.comctl32
--rw-r--r--   0 vsts      (1001) docker     (121)       91 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.credui
--rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.cryptbase
--rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.cryptdll
--rw-r--r--   0 vsts      (1001) docker     (121)       24 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.cscapi
--rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.dbghelp
--rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.devmgr
--rw-r--r--   0 vsts      (1001) docker     (121)      406 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.dnsapi
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.drprov
--rw-r--r--   0 vsts      (1001) docker     (121)      225 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.dsound
--rw-r--r--   0 vsts      (1001) docker     (121)       32 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.dsuiext
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.esent
--rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.fveapi
--rw-r--r--   0 vsts      (1001) docker     (121)      127 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.fwpuclnt
--rw-r--r--   0 vsts      (1001) docker     (121)     1913 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.gdi32
--rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.gina
--rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.icmp
--rw-r--r--   0 vsts      (1001) docker     (121)     1254 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.imagehlp
--rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.iphlpapi
--rw-r--r--   0 vsts      (1001) docker     (121)    19404 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.kernel32
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.kernelbase
--rw-r--r--   0 vsts      (1001) docker     (121)     2218 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.libeay32
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.lsasrv
--rw-r--r--   0 vsts      (1001) docker     (121)      265 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mapi32
--rw-r--r--   0 vsts      (1001) docker     (121)     1968 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mfc42
--rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mpr
--rw-r--r--   0 vsts      (1001) docker     (121)      143 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mprapi
--rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msacm32
--rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msasn1
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mscoree
--rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msi
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msimg32
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mspdb80
--rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mssign32
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msutb
--rw-r--r--   0 vsts      (1001) docker     (121)     1527 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msvbvm60
--rw-r--r--   0 vsts      (1001) docker     (121)     3448 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msvcrt
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.msvfw32
--rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mswsock
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.mydocs
--rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.nddeapi
--rw-r--r--   0 vsts      (1001) docker     (121)     1276 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.netapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.netplwiz
--rw-r--r--   0 vsts      (1001) docker     (121)     4660 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ntdll
--rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ntdsapi
--rw-r--r--   0 vsts      (1001) docker     (121)     1137 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ntoskrnl
--rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ntshrui
--rw-r--r--   0 vsts      (1001) docker     (121)     1599 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.odbc32
--rw-r--r--   0 vsts      (1001) docker     (121)      970 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.odbccp32
--rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.odbctrac
--rw-r--r--   0 vsts      (1001) docker     (121)      829 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ole32
--rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.oleaut32
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.oledlg
--rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.onex
--rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.packet
--rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.pdh
--rw-r--r--   0 vsts      (1001) docker     (121)     2236 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.powrprof
--rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.psapi
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.pstorec
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.query
--rw-r--r--   0 vsts      (1001) docker     (121)       29 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.rasapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.rastapi
--rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.riched20
--rw-r--r--   0 vsts      (1001) docker     (121)     1207 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.rpcrt4
--rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.scarddlg
--rw-r--r--   0 vsts      (1001) docker     (121)     1561 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.scecli
--rw-r--r--   0 vsts      (1001) docker     (121)      729 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.se
--rw-r--r--   0 vsts      (1001) docker     (121)      166 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.secur32
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.sensapi
--rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.setupapi
--rw-r--r--   0 vsts      (1001) docker     (121)      123 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.sfc
--rw-r--r--   0 vsts      (1001) docker     (121)     3672 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.shell32
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.shimgvw
--rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.shlwapi
--rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.shsvcs
--rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.ssleay32
--rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.unknown
--rw-r--r--   0 vsts      (1001) docker     (121)     1068 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.urlmon
--rw-r--r--   0 vsts      (1001) docker     (121)     1564 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.user32
--rw-r--r--   0 vsts      (1001) docker     (121)      309 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.userenv
--rw-r--r--   0 vsts      (1001) docker     (121)      114 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.usp10
--rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.version
--rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winhttp
--rw-r--r--   0 vsts      (1001) docker     (121)      928 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wininet
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winmm
--rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winscard
--rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winshfhc
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winsock
--rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winspool
--rw-r--r--   0 vsts      (1001) docker     (121)     3887 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.winsta
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wintrust
--rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wlanapi
--rw-r--r--   0 vsts      (1001) docker     (121)      249 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wldap32
--rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wship6
--rw-r--r--   0 vsts      (1001) docker     (121)      754 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wsnmp32
--rw-r--r--   0 vsts      (1001) docker     (121)      490 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/api/api.wtsapi32
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/archive
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/av.name
--rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/cryptography
--rw-r--r--   0 vsts      (1001) docker     (121)       70 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/debugger.device.name
--rw-r--r--   0 vsts      (1001) docker     (121)      168 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/enable_content
--rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/environment.windows
--rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/event
--rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/guid
--rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/key
--rw-r--r--   0 vsts      (1001) docker     (121)       41 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/network.protocol
--rw-r--r--   0 vsts      (1001) docker     (121)      532 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/network.string
--rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/oid
--rw-r--r--   0 vsts      (1001) docker     (121)     2674 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/os_name
--rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/powershell.cmdlet
--rw-r--r--   0 vsts      (1001) docker     (121)      873 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/privilege
--rw-r--r--   0 vsts      (1001) docker     (121)     1038 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/ransomware.string
--rw-r--r--   0 vsts      (1001) docker     (121)      263 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/sandbox.id
--rw-r--r--   0 vsts      (1001) docker     (121)      902 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/security_identifier
--rw-r--r--   0 vsts      (1001) docker     (121)      151 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/user_agent
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/vba.name
--rw-r--r--   0 vsts      (1001) docker     (121)     2164 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords/windows.registry
--rw-r--r--   0 vsts      (1001) docker     (121)    22786 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/keywords_to_review.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2634 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1410 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/query.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2277 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/registry.py
--rw-r--r--   0 vsts      (1001) docker     (121)      472 2022-04-28 15:56:20.000000 multidecoder-0.0.8/multidecoder/string_helper.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.432037 multidecoder-0.0.8/multidecoder.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-04-28 15:57:20.000000 multidecoder-0.0.8/multidecoder.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     6193 2022-04-28 15:57:21.000000 multidecoder-0.0.8/multidecoder.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-04-28 15:57:20.000000 multidecoder-0.0.8/multidecoder.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-04-28 15:57:21.000000 multidecoder-0.0.8/multidecoder.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-04-28 15:56:30.000000 multidecoder-0.0.8/multidecoder.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-04-28 15:57:21.000000 multidecoder-0.0.8/multidecoder.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-04-28 15:57:21.000000 multidecoder-0.0.8/multidecoder.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.444037 multidecoder-0.0.8/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (121)     1252 2022-04-28 15:56:20.000000 multidecoder-0.0.8/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-04-28 15:56:20.000000 multidecoder-0.0.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-04-28 15:57:21.448037 multidecoder-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)       69 2022-04-28 15:56:20.000000 multidecoder-0.0.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.448037 multidecoder-0.0.8/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-04-28 15:57:21.448037 multidecoder-0.0.8/tests/test_analyzers/
--rw-r--r--   0 vsts      (1001) docker     (121)     1020 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_base64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1927 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_concat.py
--rw-r--r--   0 vsts      (1001) docker     (121)      567 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_encoding.py
--rw-r--r--   0 vsts      (1001) docker     (121)      334 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_filename.py
--rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_hex.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_network.py
--rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_path.py
--rw-r--r--   0 vsts      (1001) docker     (121)      382 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_pe_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2747 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_shell.py
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_vba.py
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_analyzers/test_xml.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1170 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tests/test_multidecoder.py
--rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-04-28 15:56:20.000000 multidecoder-0.0.8/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2126 2022-05-03 17:11:59.000000 multidecoder-0.0.9/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-05-03 17:11:59.000000 multidecoder-0.0.9/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-05-03 17:13:01.612146 multidecoder-0.0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1657 2022-05-03 17:11:59.000000 multidecoder-0.0.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.592146 multidecoder-0.0.9/multidecoder/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      142 2022-05-03 17:13:00.000000 multidecoder-0.0.9/multidecoder/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.596146 multidecoder-0.0.9/multidecoder/analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1816 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/base64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/concat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      444 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/filename.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/hex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3930 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/network.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/path.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4396 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/shell.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1108 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/vba.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/analyzers/xml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22373 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/domains.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      808 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/hit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1987 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/json_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1067 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keyword.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.596146 multidecoder-0.0.9/multidecoder/keywords/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/multidecoder/keywords/api/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4040 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.advapi32
+-rw-r--r--   0 vsts      (1001) docker     (121)       23 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.apphelp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1212 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl
+-rw-r--r--   0 vsts      (1001) docker     (121)      243 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl80
+-rw-r--r--   0 vsts      (1001) docker     (121)      229 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.atl90
+-rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.au3zip
+-rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.avicap32
+-rw-r--r--   0 vsts      (1001) docker     (121)      196 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cabinet
+-rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.clbcatq
+-rw-r--r--   0 vsts      (1001) docker     (121)       56 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cmdial32
+-rw-r--r--   0 vsts      (1001) docker     (121)      177 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.comctl32
+-rw-r--r--   0 vsts      (1001) docker     (121)       91 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.credui
+-rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cryptbase
+-rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cryptdll
+-rw-r--r--   0 vsts      (1001) docker     (121)       24 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.cscapi
+-rw-r--r--   0 vsts      (1001) docker     (121)      610 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dbghelp
+-rw-r--r--   0 vsts      (1001) docker     (121)       79 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.devmgr
+-rw-r--r--   0 vsts      (1001) docker     (121)      406 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dnsapi
+-rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.drprov
+-rw-r--r--   0 vsts      (1001) docker     (121)      225 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dsound
+-rw-r--r--   0 vsts      (1001) docker     (121)       32 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.dsuiext
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.esent
+-rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.fveapi
+-rw-r--r--   0 vsts      (1001) docker     (121)      127 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.fwpuclnt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1913 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.gdi32
+-rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.gina
+-rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.icmp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1254 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.imagehlp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.iphlpapi
+-rw-r--r--   0 vsts      (1001) docker     (121)    19404 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.kernel32
+-rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.kernelbase
+-rw-r--r--   0 vsts      (1001) docker     (121)     2218 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.libeay32
+-rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.lsasrv
+-rw-r--r--   0 vsts      (1001) docker     (121)      265 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mapi32
+-rw-r--r--   0 vsts      (1001) docker     (121)     1968 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mfc42
+-rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mpr
+-rw-r--r--   0 vsts      (1001) docker     (121)      143 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mprapi
+-rw-r--r--   0 vsts      (1001) docker     (121)       54 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msacm32
+-rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msasn1
+-rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mscoree
+-rw-r--r--   0 vsts      (1001) docker     (121)     4043 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msi
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msimg32
+-rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mspdb80
+-rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mssign32
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msutb
+-rw-r--r--   0 vsts      (1001) docker     (121)     1527 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvbvm60
+-rw-r--r--   0 vsts      (1001) docker     (121)     3448 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvcrt
+-rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.msvfw32
+-rw-r--r--   0 vsts      (1001) docker     (121)       16 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mswsock
+-rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.mydocs
+-rw-r--r--   0 vsts      (1001) docker     (121)      525 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.nddeapi
+-rw-r--r--   0 vsts      (1001) docker     (121)     1276 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.netapi32
+-rw-r--r--   0 vsts      (1001) docker     (121)       20 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.netplwiz
+-rw-r--r--   0 vsts      (1001) docker     (121)     4660 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntdll
+-rw-r--r--   0 vsts      (1001) docker     (121)      197 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntdsapi
+-rw-r--r--   0 vsts      (1001) docker     (121)     1137 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntoskrnl
+-rw-r--r--   0 vsts      (1001) docker     (121)       43 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ntshrui
+-rw-r--r--   0 vsts      (1001) docker     (121)     1599 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbc32
+-rw-r--r--   0 vsts      (1001) docker     (121)      970 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbccp32
+-rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.odbctrac
+-rw-r--r--   0 vsts      (1001) docker     (121)      829 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ole32
+-rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.oleaut32
+-rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.oledlg
+-rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.onex
+-rw-r--r--   0 vsts      (1001) docker     (121)      587 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.packet
+-rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.pdh
+-rw-r--r--   0 vsts      (1001) docker     (121)     2236 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.powrprof
+-rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.psapi
+-rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.pstorec
+-rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.query
+-rw-r--r--   0 vsts      (1001) docker     (121)       29 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rasapi32
+-rw-r--r--   0 vsts      (1001) docker     (121)       22 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rastapi
+-rw-r--r--   0 vsts      (1001) docker     (121)       18 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.riched20
+-rw-r--r--   0 vsts      (1001) docker     (121)     1207 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.rpcrt4
+-rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.scarddlg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1561 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.scecli
+-rw-r--r--   0 vsts      (1001) docker     (121)      729 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.se
+-rw-r--r--   0 vsts      (1001) docker     (121)      166 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.secur32
+-rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.sensapi
+-rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.setupapi
+-rw-r--r--   0 vsts      (1001) docker     (121)      123 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.sfc
+-rw-r--r--   0 vsts      (1001) docker     (121)     3672 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shell32
+-rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shimgvw
+-rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shlwapi
+-rw-r--r--   0 vsts      (1001) docker     (121)       26 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.shsvcs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.ssleay32
+-rw-r--r--   0 vsts      (1001) docker     (121)       86 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.unknown
+-rw-r--r--   0 vsts      (1001) docker     (121)     1068 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.urlmon
+-rw-r--r--   0 vsts      (1001) docker     (121)     1564 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.user32
+-rw-r--r--   0 vsts      (1001) docker     (121)      309 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.userenv
+-rw-r--r--   0 vsts      (1001) docker     (121)      114 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.usp10
+-rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.version
+-rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winhttp
+-rw-r--r--   0 vsts      (1001) docker     (121)      928 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wininet
+-rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winmm
+-rw-r--r--   0 vsts      (1001) docker     (121)      219 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winscard
+-rw-r--r--   0 vsts      (1001) docker     (121)       21 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winshfhc
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winsock
+-rw-r--r--   0 vsts      (1001) docker     (121)      254 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winspool
+-rw-r--r--   0 vsts      (1001) docker     (121)     3887 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.winsta
+-rw-r--r--   0 vsts      (1001) docker     (121)       14 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wintrust
+-rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wlanapi
+-rw-r--r--   0 vsts      (1001) docker     (121)      249 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wldap32
+-rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wship6
+-rw-r--r--   0 vsts      (1001) docker     (121)      754 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wsnmp32
+-rw-r--r--   0 vsts      (1001) docker     (121)      490 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/api/api.wtsapi32
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/archive
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/av.name
+-rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/cryptography
+-rw-r--r--   0 vsts      (1001) docker     (121)       70 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/debugger.device.name
+-rw-r--r--   0 vsts      (1001) docker     (121)      168 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/enable_content
+-rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/environment.windows
+-rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/event
+-rw-r--r--   0 vsts      (1001) docker     (121)      517 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/guid
+-rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/key
+-rw-r--r--   0 vsts      (1001) docker     (121)       41 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/network.protocol
+-rw-r--r--   0 vsts      (1001) docker     (121)      532 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/network.string
+-rw-r--r--   0 vsts      (1001) docker     (121)     1812 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/oid
+-rw-r--r--   0 vsts      (1001) docker     (121)     2674 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/os_name
+-rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/powershell.cmdlet
+-rw-r--r--   0 vsts      (1001) docker     (121)      873 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/privilege
+-rw-r--r--   0 vsts      (1001) docker     (121)     1038 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/ransomware.string
+-rw-r--r--   0 vsts      (1001) docker     (121)      263 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/sandbox.id
+-rw-r--r--   0 vsts      (1001) docker     (121)      902 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/security_identifier
+-rw-r--r--   0 vsts      (1001) docker     (121)      151 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/user_agent
+-rw-r--r--   0 vsts      (1001) docker     (121)       53 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/vba.name
+-rw-r--r--   0 vsts      (1001) docker     (121)     2164 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords/windows.registry
+-rw-r--r--   0 vsts      (1001) docker     (121)    22786 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/keywords_to_review.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     2634 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1410 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/query.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2277 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      472 2022-05-03 17:11:59.000000 multidecoder-0.0.9/multidecoder/string_helper.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.592146 multidecoder-0.0.9/multidecoder.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2324 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     6193 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       60 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-03 17:12:09.000000 multidecoder-0.0.9/multidecoder.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       13 2022-05-03 17:13:01.000000 multidecoder-0.0.9/multidecoder.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1252 2022-05-03 17:11:59.000000 multidecoder-0.0.9/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (121)      239 2022-05-03 17:11:59.000000 multidecoder-0.0.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-05-03 17:13:01.612146 multidecoder-0.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)       69 2022-05-03 17:11:59.000000 multidecoder-0.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-03 17:13:01.612146 multidecoder-0.0.9/tests/test_analyzers/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1215 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_base64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1927 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_concat.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      567 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_encoding.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      334 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_filename.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_hex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4661 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_network.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_path.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      382 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_pe_file.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4561 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_shell.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_vba.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_analyzers/test_xml.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1170 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tests/test_multidecoder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      111 2022-05-03 17:11:59.000000 multidecoder-0.0.9/tox.ini
```

### Comparing `multidecoder-0.0.8/.gitignore` & `multidecoder-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/LICENSE.md` & `multidecoder-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/PKG-INFO` & `multidecoder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

### Comparing `multidecoder-0.0.8/README.md` & `multidecoder-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/__main__.py` & `multidecoder-0.0.9/multidecoder/__main__.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/base64.py` & `multidecoder-0.0.9/multidecoder/analyzers/base64.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import regex as re
 
 
 from multidecoder.hit import Hit
 from multidecoder.registry import analyzer
 
 HTML_ESCAPE_RE = rb'&#(?:x[a-fA-F0-9]{1,4}|\d{1,4});'
-BASE64_RE = rb'\b(?:[A-Za-z0-9+/]{4,}(?:<\x00  \x00)?(?:&#13;|&#xD;)?(?:&#10;|&#xA)?\r?\n?){5,}' \
-            rb'[A-Za-z0-9+/]{2,}={0,2}\b'
+BASE64_RE = rb'(?:[A-Za-z0-9+/]{4,}(?:<\x00  \x00)?(?:&#13;|&#xD;)?(?:&#10;|&#xA)?\r?\n?){5,}' \
+            rb'[A-Za-z0-9+/]{2,}=?=?'
 
 CAMEL_RE = rb'(?i)[a-z]+'
 HEX_RE = rb'(?i)[a-f0-9]+'
 MIN_B64_CHARS = 6
 
 
 @analyzer('')
```

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/concat.py` & `multidecoder-0.0.9/multidecoder/analyzers/concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/network.py` & `multidecoder-0.0.9/multidecoder/analyzers/network.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/pe_file.py` & `multidecoder-0.0.9/multidecoder/analyzers/pe_file.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/shell.py` & `multidecoder-0.0.9/multidecoder/analyzers/shell.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 CMD_RE = rb'(?i)\bc\^?m\^?d(?:' + DOUBLE_QUOTE_ESCAPES + rb'|[^)"])+'
 POWERSHELL_INDICATOR_RE = rb'(?i)(?:^|/c|/k|[\s;,=\'"])(\^?p\^?(?:o\^?w\^?e\^?r\^?s\^?h\^?e\^?l\^?l|w\^?s\^?h))\b'
 SH_RE = rb'"(\s*(?:sh|bash|zsh|csh)[^"]+)"'
 ENC_RE = rb'(?i)\s\^?(?:-|/)\^?e\^?(?:c|n\^?(?:c\^?(?:o\^?(?:d\^?(?:e\^?(?:d\^?(?:c\^?(?:o\^?(?:m' \
          rb'\^?(?:m\^?(?:a\^?(?:n\^?d?)?)?)?)?)?)?)?)?)?)?)?)?[\s^]+([a-z0-9+/^]{4,}=?\^?=?\^?)'
+POWERSHELL_ARGS_RE = rb'\s*(powershell|pwsh)?(.exe)?\s*((-|/)[^\s]+\s+)*'
 
 
 def strip_carets(cmd: bytes) -> bytes:
     in_string = False
     out = []
     i = 0
     while i < len(cmd)-1:
@@ -60,15 +61,15 @@
         if enc:
             powershell = data[start:enc.end()]
             deobfuscated, ob = deobfuscate_cmd(powershell)
             split = re.split(rb'\s+', deobfuscated)
             b64 = (binascii.a2b_base64(_pad(split[-1]))
                            .decode('utf-16', errors='ignore')
                            .encode())
-            deobfuscated = b' '.join(split[:-2]) + b' ' + b64
+            deobfuscated = b' '.join(split[:-2]) + b' -Command ' + b64
             obfuscation = ob + ('/>' if ob else '') + 'powershell.base64'
             out.append(Hit(deobfuscated, obfuscation, start, enc.end()))
             continue
         # Look back to find the start of the string or FOR loop
         bound_match = re.search(rb'(\'\(|[\'"])', data[start::-1])
         if bound_match:
             bound = bound_match.group()
@@ -96,7 +97,33 @@
     padding = -len(b64) % 4
     if padding == 3:
         return b64[:-1]  # Corrupted end, just keep the valid part
     elif padding:
         return b64 + b'='*padding
     else:
         return b64
+
+
+def get_cmd_command(cmd: bytes):
+    # Find end of argument string
+    lcmd = cmd.lower()
+    arg_end = len(cmd)
+    c = lcmd.find(b'/c')
+    if c > 0:
+        arg_end = min(arg_end, c+2)
+    k = lcmd.find(b'/k')
+    if k > 0:
+        arg_end = min(arg_end, k+2)
+    amp = lcmd.find(b'&')
+    if amp > 0:
+        arg_end = min(arg_end, amp+1)
+
+    # return everything after the arguments
+    return cmd[arg_end:]
+
+
+def get_powershell_command(powershell: bytes):
+    match = re.match(POWERSHELL_ARGS_RE, powershell)
+    if match:
+        return powershell[match.end():]
+    else:
+        return powershell
```

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/vba.py` & `multidecoder-0.0.9/multidecoder/analyzers/vba.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/analyzers/xml.py` & `multidecoder-0.0.9/multidecoder/analyzers/xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/domains.py` & `multidecoder-0.0.9/multidecoder/domains.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/hit.py` & `multidecoder-0.0.9/multidecoder/hit.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/json_conversion.py` & `multidecoder-0.0.9/multidecoder/json_conversion.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keyword.py` & `multidecoder-0.0.9/multidecoder/keyword.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.advapi32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.advapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.atl` & `multidecoder-0.0.9/multidecoder/keywords/api/api.atl`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.dbghelp` & `multidecoder-0.0.9/multidecoder/keywords/api/api.dbghelp`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.gdi32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.gdi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.imagehlp` & `multidecoder-0.0.9/multidecoder/keywords/api/api.imagehlp`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.iphlpapi` & `multidecoder-0.0.9/multidecoder/keywords/api/api.iphlpapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.kernel32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.kernel32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.libeay32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.libeay32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.mfc42` & `multidecoder-0.0.9/multidecoder/keywords/api/api.mfc42`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.msi` & `multidecoder-0.0.9/multidecoder/keywords/api/api.msi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.mssign32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.mssign32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.msvbvm60` & `multidecoder-0.0.9/multidecoder/keywords/api/api.msvbvm60`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.msvcrt` & `multidecoder-0.0.9/multidecoder/keywords/api/api.msvcrt`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.nddeapi` & `multidecoder-0.0.9/multidecoder/keywords/api/api.nddeapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.netapi32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.netapi32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.ntdll` & `multidecoder-0.0.9/multidecoder/keywords/api/api.ntdll`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.ntoskrnl` & `multidecoder-0.0.9/multidecoder/keywords/api/api.ntoskrnl`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.odbc32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.odbc32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.odbccp32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.odbccp32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.ole32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.ole32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.oleaut32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.oleaut32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.packet` & `multidecoder-0.0.9/multidecoder/keywords/api/api.packet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.powrprof` & `multidecoder-0.0.9/multidecoder/keywords/api/api.powrprof`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.rpcrt4` & `multidecoder-0.0.9/multidecoder/keywords/api/api.rpcrt4`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.scecli` & `multidecoder-0.0.9/multidecoder/keywords/api/api.scecli`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.se` & `multidecoder-0.0.9/multidecoder/keywords/api/api.se`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.shell32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.shell32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.shlwapi` & `multidecoder-0.0.9/multidecoder/keywords/api/api.shlwapi`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.ssleay32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.ssleay32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.urlmon` & `multidecoder-0.0.9/multidecoder/keywords/api/api.urlmon`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.user32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.user32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.wininet` & `multidecoder-0.0.9/multidecoder/keywords/api/api.wininet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.winsock` & `multidecoder-0.0.9/multidecoder/keywords/api/api.winsock`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.winsta` & `multidecoder-0.0.9/multidecoder/keywords/api/api.winsta`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/api/api.wsnmp32` & `multidecoder-0.0.9/multidecoder/keywords/api/api.wsnmp32`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/event` & `multidecoder-0.0.9/multidecoder/keywords/event`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/guid` & `multidecoder-0.0.9/multidecoder/keywords/guid`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/key` & `multidecoder-0.0.9/multidecoder/keywords/key`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/network.string` & `multidecoder-0.0.9/multidecoder/keywords/network.string`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/oid` & `multidecoder-0.0.9/multidecoder/keywords/oid`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/os_name` & `multidecoder-0.0.9/multidecoder/keywords/os_name`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/powershell.cmdlet` & `multidecoder-0.0.9/multidecoder/keywords/powershell.cmdlet`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/privilege` & `multidecoder-0.0.9/multidecoder/keywords/privilege`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/ransomware.string` & `multidecoder-0.0.9/multidecoder/keywords/ransomware.string`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/security_identifier` & `multidecoder-0.0.9/multidecoder/keywords/security_identifier`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords/windows.registry` & `multidecoder-0.0.9/multidecoder/keywords/windows.registry`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/keywords_to_review.txt` & `multidecoder-0.0.9/multidecoder/keywords_to_review.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/multidecoder.py` & `multidecoder-0.0.9/multidecoder/multidecoder.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/query.py` & `multidecoder-0.0.9/multidecoder/query.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder/registry.py` & `multidecoder-0.0.9/multidecoder/registry.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/multidecoder.egg-info/PKG-INFO` & `multidecoder-0.0.9/multidecoder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidecoder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A context preserving IOC extraction library
 Home-page: https://github.com/CybercentreCanada/Multidecoder
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CybercentreCanada/Multidecoder/issues
 Keywords: malware,analysis,gc,canada,cse-cst,cse,cst,cyber,cccs
```

### Comparing `multidecoder-0.0.8/multidecoder.egg-info/SOURCES.txt` & `multidecoder-0.0.9/multidecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/pipelines/publish.yaml` & `multidecoder-0.0.9/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/setup.cfg` & `multidecoder-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_base64.py` & `multidecoder-0.0.9/tests/test_analyzers/test_base64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import binascii
+import regex as re
 
-from multidecoder.analyzers.base64 import find_base64
+from multidecoder.analyzers.base64 import find_base64, BASE64_RE
 
 
 def test_empty():
     assert find_base64(b'') == []
 
 
 def test_hex():
@@ -17,14 +18,21 @@
     assert find_base64(b'WakeAllConditionVariable, GetUserDefaultUILanguage') == []
 
 
 def test_url():
     assert find_base64(b'http://schemas.microsoft.com/SMI/2016/WindowsSettings') == []
 
 
+def test_base64_re_matches_equals():
+    ex = b'bmljZSBkYXksIGlzbid0IGl0Pw=='
+    match = re.search(BASE64_RE, ex)
+    assert match
+    assert match.group() == ex
+
+
 ENCODED = binascii.b2a_base64(b'Some base64 encoded text')
 TEST_STRINGS = {
     ENCODED: [(b'Some base64 encoded text', 'decoded.base64', 0, 32)],
     b'lorem ipsum lorum asdf\nhjkl\nASDF\nasdf\nhjkl\nASDF\n44==lorum ipsum':
         [(b'j\xc7_\x869%\x01 \xc5j\xc7_\x869%\x01 \xc5\xe3', 'decoded.base64', 18, 52)]
 }
```

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_concat.py` & `multidecoder-0.0.9/tests/test_analyzers/test_concat.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_encoding.py` & `multidecoder-0.0.9/tests/test_analyzers/test_encoding.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_network.py` & `multidecoder-0.0.9/tests/test_analyzers/test_network.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_path.py` & `multidecoder-0.0.9/tests/test_analyzers/test_path.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_analyzers/test_xml.py` & `multidecoder-0.0.9/tests/test_analyzers/test_xml.py`

 * *Files identical despite different names*

### Comparing `multidecoder-0.0.8/tests/test_multidecoder.py` & `multidecoder-0.0.9/tests/test_multidecoder.py`

 * *Files identical despite different names*

