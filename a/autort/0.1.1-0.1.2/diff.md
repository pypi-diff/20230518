# Comparing `tmp/autort-0.1.1-cp38-cp38-win_amd64.whl.zip` & `tmp/autort-0.1.2-cp38-cp38-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   9740216 (0000000000949FB8h)
-  Actual end-cent-dir record offset:       9740194 (0000000000949FA2h)
-  Expected end-cent-dir record offset:     9740194 (0000000000949FA2h)
+  Zip archive file size:                   9824206 (000000000095E7CEh)
+  Actual end-cent-dir record offset:       9824184 (000000000095E7B8h)
+  Expected end-cent-dir record offset:     9824184 (000000000095E7B8h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 21 entries.
-  The central directory is 2306 (0000000000000902h) bytes long,
+  central directory contains 31 entries.
+  The central directory is 3371 (0000000000000D2Bh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 9737888 (00000000009496A0h).
+  is 9820813 (000000000095DA8Dh).
 
 
 Central directory entry #1:
 ---------------------------
 
   autort/
 
@@ -48,25 +48,94 @@
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort/lib/
+  autort/examples/
 
   offset of local header from start of archive:   37
                                                   (0000000000000025h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 18 17:00:58
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             16 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 50 69 9d 42 67 89 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #3:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/examples/mnist.py
+
+  offset of local header from start of archive:   83
+                                                  (0000000000000053h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 18 17:30:50
+  32-bit CRC value (hex):                         483ef08e
+  compressed size:                                1077 bytes
+  uncompressed size:                              3288 bytes
+  length of filename:                             24 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 14 87 c0 6e 6b 89 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #4:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/lib/
+
+  offset of local header from start of archive:   1214
+                                                  (00000000000004BEh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
   file last modified on (DOS date/time):          2023 May 16 20:03:10
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             11 characters
   length of extra field:                          36 bytes
   length of file comment:                         0 characters
@@ -77,58 +146,58 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 6b d3 5d 61 ee 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #5:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/lib/antares_backend.cp38-win_amd64.pyd
 
-  offset of local header from start of archive:   78
-                                                  (000000000000004Eh) bytes
+  offset of local header from start of archive:   1255
+                                                  (00000000000004E7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 23:17:24
-  32-bit CRC value (hex):                         0f04a345
-  compressed size:                                125384 bytes
-  uncompressed size:                              330240 bytes
+  file last modified on (DOS date/time):          2023 May 18 16:50:38
+  32-bit CRC value (hex):                         c47b627c
+  compressed size:                                137000 bytes
+  uncompressed size:                              371200 bytes
   length of filename:                             45 characters
   length of extra field:                          36 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
-    20 are:   00 00 00 00 01 00 18 00 2a 2c d4 83 09 88 d9 01 00 00 00 00.
+    20 are:   00 00 00 00 01 00 18 00 a2 c6 63 d0 65 89 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #6:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/lib/antares_hlsl_v0.3.4_x64.dll
 
-  offset of local header from start of archive:   125537
-                                                  (000000000001EA61h) bytes
+  offset of local header from start of archive:   138330
+                                                  (0000000000021C5Ah) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -147,23 +216,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 2e 49 be e3 08 6b d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #7:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/lib/antares_hlsl_xbox_v0.3.4_x64.dll
 
-  offset of local header from start of archive:   388056
-                                                  (000000000005EBD8h) bytes
+  offset of local header from start of archive:   400849
+                                                  (0000000000061DD1h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -182,23 +251,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 13 c4 d1 31 7c 6a d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #8:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/lib/dxcompiler.dll
 
-  offset of local header from start of archive:   443698
-                                                  (000000000006C532h) bytes
+  offset of local header from start of archive:   456491
+                                                  (000000000006F72Bh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -217,23 +286,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 76 47 cd e3 08 6b d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #9:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/lib/dxil.dll
 
-  offset of local header from start of archive:   9018253
-                                                  (0000000000899B8Dh) bytes
+  offset of local header from start of archive:   9031046
+                                                  (000000000089CD86h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -252,23 +321,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 76 47 cd e3 08 6b d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #10:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/ops/
 
-  offset of local header from start of archive:   9697609
-                                                  (000000000093F949h) bytes
+  offset of local header from start of archive:   9710402
+                                                  (0000000000942B42h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -286,58 +355,128 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 90 49 d9 26 eb 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #11:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/addmm_fp32.mod
+
+  offset of local header from start of archive:   9710443
+                                                  (0000000000942B6Bh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 18 17:04:04
+  32-bit CRC value (hex):                         d590ef00
+  compressed size:                                7523 bytes
+  uncompressed size:                              12596 bytes
+  length of filename:                             25 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 f4 8e b2 b0 67 89 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #12:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/ops/fill_C8.mod
 
-  offset of local header from start of archive:   9697650
-                                                  (000000000093F972h) bytes
+  offset of local header from start of archive:   9718021
+                                                  (0000000000944905h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Apr 15 23:02:00
-  32-bit CRC value (hex):                         b9703ea0
-  compressed size:                                3381 bytes
-  uncompressed size:                              5416 bytes
+  file last modified on (DOS date/time):          2023 May 17 20:31:40
+  32-bit CRC value (hex):                         59f29d50
+  compressed size:                                3124 bytes
+  uncompressed size:                              5635 bytes
   length of filename:                             22 characters
   length of extra field:                          36 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
-    20 are:   00 00 00 00 01 00 18 00 50 ee bb 3a ab 6f d9 01 00 00 00 00.
+    20 are:   00 00 00 00 01 00 18 00 22 8f fc 86 bb 88 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #13:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/ops/gemm_nn_fp32.mod
 
-  offset of local header from start of archive:   9701083
-                                                  (00000000009406DBh) bytes
+  offset of local header from start of archive:   9721197
+                                                  (000000000094556Dh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 18:02:40
+  32-bit CRC value (hex):                         3178886f
+  compressed size:                                37503 bytes
+  uncompressed size:                              66044 bytes
+  length of filename:                             27 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 54 14 cd b6 a6 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #14:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/gemm_tn_fp32.mod
+
+  offset of local header from start of archive:   9758757
+                                                  (000000000094E825h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -356,58 +495,268 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 6d 23 72 74 5f 88 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #15:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/log_fp32.mod
+
+  offset of local header from start of archive:   9792822
+                                                  (0000000000956D36h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 17:01:28
+  32-bit CRC value (hex):                         d3f4fe6f
+  compressed size:                                3651 bytes
+  uncompressed size:                              6041 bytes
+  length of filename:                             23 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 a4 e4 41 2a 9e 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #16:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/max_fp32.mod
+
+  offset of local header from start of archive:   9796526
+                                                  (0000000000957BAEh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 17:00:34
+  32-bit CRC value (hex):                         3f8be435
+  compressed size:                                4250 bytes
+  uncompressed size:                              7008 bytes
+  length of filename:                             23 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 1a 07 36 09 9e 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #17:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/nll_loss_fp32.mod
+
+  offset of local header from start of archive:   9800829
+                                                  (0000000000958C7Dh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 18 00:00:12
+  32-bit CRC value (hex):                         00e7beb6
+  compressed size:                                3728 bytes
+  uncompressed size:                              7225 bytes
+  length of filename:                             28 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 47 20 91 a8 d8 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #18:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/relu_fp32.mod
+
+  offset of local header from start of archive:   9804615
+                                                  (0000000000959B47h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 16:13:40
+  32-bit CRC value (hex):                         541c7a36
+  compressed size:                                3821 bytes
+  uncompressed size:                              6019 bytes
+  length of filename:                             24 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 ce cb ed 7b 97 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #19:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/softmax_post_fp32.mod
+
+  offset of local header from start of archive:   9808490
+                                                  (000000000095AA6Ah) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 17:33:36
+  32-bit CRC value (hex):                         65c1cbd3
+  compressed size:                                5203 bytes
+  uncompressed size:                              8203 bytes
+  length of filename:                             32 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 45 4d 40 a7 a2 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #20:
+---------------------------
+
+  There are an extra -36 bytes preceding this file.
+
+  autort/ops/sum_fp32.mod
+
+  offset of local header from start of archive:   9813755
+                                                  (000000000095BEFBh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   6.3
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 17 23:34:20
+  32-bit CRC value (hex):                         854c1cc9
+  compressed size:                                4174 bytes
+  uncompressed size:                              6856 bytes
+  length of filename:                             23 characters
+  length of extra field:                          36 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
+    20 are:   00 00 00 00 01 00 18 00 41 01 2e 0c d5 88 d9 01 00 00 00 00.
+
+  There is no file comment.
+
+Central directory entry #21:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
   autort/__init__.py
 
-  offset of local header from start of archive:   9735148
-                                                  (0000000000948BECh) bytes
+  offset of local header from start of archive:   9817982
+                                                  (000000000095CF7Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 16 21:54:58
-  32-bit CRC value (hex):                         7468fbc9
-  compressed size:                                946 bytes
-  uncompressed size:                              2080 bytes
+  file last modified on (DOS date/time):          2023 May 18 17:02:46
+  32-bit CRC value (hex):                         99a2ba4f
+  compressed size:                                1037 bytes
+  uncompressed size:                              2376 bytes
   length of filename:                             18 characters
   length of extra field:                          36 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
-    20 are:   00 00 00 00 01 00 18 00 39 14 88 ff fd 87 d9 01 00 00 00 00.
+    20 are:   00 00 00 00 01 00 18 00 d4 a8 17 82 67 89 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #22:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/
+  autort-0.1.2.dist-info/
 
-  offset of local header from start of archive:   9736142
-                                                  (0000000000948FCEh) bytes
+  offset of local header from start of archive:   9819067
+                                                  (000000000095D3BBh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -425,23 +774,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 9d b2 b9 af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #23:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/direct_url.json
+  autort-0.1.2.dist-info/direct_url.json
 
-  offset of local header from start of archive:   9736195
-                                                  (0000000000949003h) bytes
+  offset of local header from start of archive:   9819120
+                                                  (000000000095D3F0h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -459,23 +808,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 e6 51 9d af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #24:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/entry_points.txt
+  autort-0.1.2.dist-info/entry_points.txt
 
-  offset of local header from start of archive:   9736331
-                                                  (000000000094908Bh) bytes
+  offset of local header from start of archive:   9819256
+                                                  (000000000095D478h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -493,23 +842,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 55 b4 28 cd ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #25:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/INSTALLER
+  autort-0.1.2.dist-info/INSTALLER
 
-  offset of local header from start of archive:   9736444
-                                                  (00000000009490FCh) bytes
+  offset of local header from start of archive:   9819369
+                                                  (000000000095D4E9h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -527,23 +876,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 d5 d8 a7 af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #26:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/LICENSE
+  autort-0.1.2.dist-info/LICENSE
 
-  offset of local header from start of archive:   9736510
-                                                  (000000000094913Eh) bytes
+  offset of local header from start of archive:   9819435
+                                                  (000000000095D52Bh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -562,58 +911,58 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 a3 13 a3 af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #27:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/METADATA
+  autort-0.1.2.dist-info/METADATA
 
-  offset of local header from start of archive:   9737225
-                                                  (0000000000949409h) bytes
+  offset of local header from start of archive:   9820150
+                                                  (000000000095D7F6h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 17 09:35:44
-  32-bit CRC value (hex):                         1ae1116c
+  file last modified on (DOS date/time):          2023 May 17 14:42:22
+  32-bit CRC value (hex):                         3e1ff932
   compressed size:                                251 bytes
   uncompressed size:                              402 bytes
   length of filename:                             31 characters
   length of extra field:                          36 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
-    20 are:   00 00 00 00 01 00 18 00 fe 63 8f e5 5f 88 d9 01 00 00 00 00.
+    20 are:   00 00 00 00 01 00 18 00 23 c2 95 ba 8a 88 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #28:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/RECORD
+  autort-0.1.2.dist-info/RECORD
 
-  offset of local header from start of archive:   9737537
-                                                  (0000000000949541h) bytes
+  offset of local header from start of archive:   9820462
+                                                  (000000000095D92Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -631,23 +980,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 6e ae bb af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #19:
+Central directory entry #29:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/REQUESTED
+  autort-0.1.2.dist-info/REQUESTED
 
-  offset of local header from start of archive:   9737596
-                                                  (000000000094957Ch) bytes
+  offset of local header from start of archive:   9820521
+                                                  (000000000095D969h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -665,23 +1014,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 41 76 a5 af ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #20:
+Central directory entry #30:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/top_level.txt
+  autort-0.1.2.dist-info/top_level.txt
 
-  offset of local header from start of archive:   9737658
-                                                  (00000000009495BAh) bytes
+  offset of local header from start of archive:   9820583
+                                                  (000000000095D9A7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -699,23 +1048,23 @@
 
   The central-directory extra field contains:
   - A subfield with ID 0x000a (PKWARE Win32) and 32 data bytes.  The first
     20 are:   00 00 00 00 01 00 18 00 af 50 ff d6 ef 87 d9 01 00 00 00 00.
 
   There is no file comment.
 
-Central directory entry #21:
+Central directory entry #31:
 ---------------------------
 
   There are an extra -36 bytes preceding this file.
 
-  autort-0.1.1.dist-info/WHEEL
+  autort-0.1.2.dist-info/WHEEL
 
-  offset of local header from start of archive:   9737731
-                                                  (0000000000949603h) bytes
+  offset of local header from start of archive:   9820656
+                                                  (000000000095D9F0h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   6.3
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
```

## zipnote {}

```diff
@@ -1,10 +1,16 @@
 Filename: autort/
 Comment: 
 
+Filename: autort/examples/
+Comment: 
+
+Filename: autort/examples/mnist.py
+Comment: 
+
 Filename: autort/lib/
 Comment: 
 
 Filename: autort/lib/antares_backend.cp38-win_amd64.pyd
 Comment: 
 
 Filename: autort/lib/antares_hlsl_v0.3.4_x64.dll
@@ -18,47 +24,71 @@
 
 Filename: autort/lib/dxil.dll
 Comment: 
 
 Filename: autort/ops/
 Comment: 
 
+Filename: autort/ops/addmm_fp32.mod
+Comment: 
+
 Filename: autort/ops/fill_C8.mod
 Comment: 
 
 Filename: autort/ops/gemm_nn_fp32.mod
 Comment: 
 
+Filename: autort/ops/gemm_tn_fp32.mod
+Comment: 
+
+Filename: autort/ops/log_fp32.mod
+Comment: 
+
+Filename: autort/ops/max_fp32.mod
+Comment: 
+
+Filename: autort/ops/nll_loss_fp32.mod
+Comment: 
+
+Filename: autort/ops/relu_fp32.mod
+Comment: 
+
+Filename: autort/ops/softmax_post_fp32.mod
+Comment: 
+
+Filename: autort/ops/sum_fp32.mod
+Comment: 
+
 Filename: autort/__init__.py
 Comment: 
 
-Filename: autort-0.1.1.dist-info/
+Filename: autort-0.1.2.dist-info/
 Comment: 
 
-Filename: autort-0.1.1.dist-info/direct_url.json
+Filename: autort-0.1.2.dist-info/direct_url.json
 Comment: 
 
-Filename: autort-0.1.1.dist-info/entry_points.txt
+Filename: autort-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: autort-0.1.1.dist-info/INSTALLER
+Filename: autort-0.1.2.dist-info/INSTALLER
 Comment: 
 
-Filename: autort-0.1.1.dist-info/LICENSE
+Filename: autort-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: autort-0.1.1.dist-info/METADATA
+Filename: autort-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: autort-0.1.1.dist-info/RECORD
+Filename: autort-0.1.2.dist-info/RECORD
 Comment: 
 
-Filename: autort-0.1.1.dist-info/REQUESTED
+Filename: autort-0.1.2.dist-info/REQUESTED
 Comment: 
 
-Filename: autort-0.1.1.dist-info/top_level.txt
+Filename: autort-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: autort-0.1.1.dist-info/WHEEL
+Filename: autort-0.1.2.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## autort/ops/fill_C8.mod

```diff
@@ -1,10 +1,10 @@
-fill_C8|blockIdx.x=1048577;threadIdx.x=1;cbuffers=3;$=1;$$=1;$0=-1;$1=1|arg_0=:0:int64;arg_1=:1:int32;o_type=infer:int64:#1||@VER__1|// GLOBALS:  -> output0:int64[1048577]
+fill_C8|blockIdx.x=513;threadIdx.x=64;cbuffers=3;$=1;$$=1;$0=-1;$1=2048|arg_0=:0:int64;arg_1=:1:int32;o_type=infer:int64:#1|-||@VER__1|// GLOBALS:  -> output0:int64[1048577]
 // BACKEND: c-hlsl_win64 (default)
-// CONFIG: null
+// CONFIG: {"N": [-1, 32, 64, 1], "UN": 1, "UK": 0, "RV": 0}
 // COMPUTE_V1: - X = 1024 * 1024 + 1; einstein_v2(f"output0[N] = const(1, dtype=`int64`).alter(`V`) where N in X:{X}", input_dict={}, func_name="fill_C8")
 
 
 // ---------------------------------------------------------------------------
 // LOCAL: fill_C8 --  -> output0:int64[1048577]
 
-@@PACK:1048577@@1@@1@@int64_t/_V:1,int/_X:1048577@@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
+@@PACK:513@@1@@1@@int64_t/_V:1,int/_X:1048577@@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
```

## autort/ops/gemm_nn_fp32.mod

```diff
@@ -1,10 +1,10 @@
-gemm_nn_fp32|blockIdx.x=4096;threadIdx.x=64;cbuffers=3;$=3;$$=1;$0=-1;$1=64;$2=64|arg_0=0:0:int32;arg_1=1:1:int32;arg_2=0:1:int32;o_type=infer:float32:#2,#1|2:float32,2:float32||@VER__1|// GLOBALS: input0:float32[4096, 4096], input1:float32[4096, 4096] -> output0:float32[4096, 4096]
+gemm_nn_fp32|blockIdx.x=2048;threadIdx.x=128;cbuffers=3;$=3;$$=1;$0=-1;$1=64;$2=128|arg_0=0:1:int32;arg_1=1:1:int32;arg_2=0:0:int32;o_type=infer:float32:#2,#1|2:float32,2:float32||@VER__1|// GLOBALS: input0:float32[4096, 4096], input1:float32[4096, 4096] -> output0:float32[4096, 4096]
 // BACKEND: c-hlsl_win64 (default)
-// CONFIG: {"N": [-1, 8, 8, 1], "M": [-1, 8, 8, 1], "K": [-1, 4, 1], "@input1": 0, "@input0": 1, "UN": 1, "UK": 1, "RV": 1}
-// COMPUTE_V1: - N, M, K = "N:4096", "M:4096", "K:4096"; einstein_v2(input_dict={"input0": {"dtype": "float32", "shape": [K, N]}, "input1": {"dtype": "float32", "shape": [K, M]}}, exprss=f"output0[N, M] +=! input0[K, N] * input1[K, M] where K in {K}", func_name="gemm_nn_fp32")
+// CONFIG: {"N": [-1, 8, 16, 1], "M": [-1, 8, 8, 1], "K": [-1, 16, 1], "@input0": 1, "@input1": 1, "UN": 1, "UK": 0, "RV": 0}
+// COMPUTE_V1: - N, M, K = "N:4096", "M:4096", "K:4096"; einstein_v2(input_dict={"input0": {"dtype": "float32", "shape": [N, K]}, "input1": {"dtype": "float32", "shape": [K, M]}}, exprss=f"output0[N, M] +=! input0[N, K] * input1[K, M] where K in {K}", func_name="gemm_nn_fp32")
 
 
 // ---------------------------------------------------------------------------
 // LOCAL: gemm_nn_fp32 -- input0:float32[4096, 4096], input1:float32[4096, 4096] -> output0:float32[4096, 4096]
 
-@@PACK:4096@@1@@1@@int/_K:4096,int/_M:4096,int/_N:4096@@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
+@@PACK:2048@@1@@1@@int/_K:4096,int/_M:4096,int/_N:4096@@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
```

## autort/__init__.py

```diff
@@ -1,14 +1,14 @@
-#!/usr/bin/env python3
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 import ctypes
 import os
 import sys
+import time
 
 try:
   import torch
   torch_version = torch.version.__version__
 except:
   torch_version = ''
 
@@ -40,15 +40,14 @@
   import numpy as np
   return torch.tensor(np.load(path), device=device())
 
 def to_npy(x, path):
   import numpy as np
   np.save(path, x.cpu().numpy())
 
-
 class OpClass:
   aops = torch.ops.antares_ops
   op_dict = {}
 
   def __getattr__(self, name: str):
     addr = id(name)
     if addr not in OpClass.op_dict:
@@ -65,14 +64,32 @@
 
 int16 = torch.int16
 int32 = torch.int32
 int64 = torch.int64
 float32 = torch.float32
 float64 = torch.float64
 
+
+import atexit
+atexit.register(lambda *_: ops.aops.control(0))
+
+def wait():
+  ops.aops.control(1)
+  return time.time()
+
+def profile():
+  class Prof():
+    def __enter__(self):
+      ops.aops.control(2)
+
+    def __exit__(self, type, value, trace):
+      ops.aops.control(3)
+  return Prof()
+
+
 ''' py
 
   # Example:
   import autort as art
 
   x = art.full([2, 4], 1.2)
   art.print(x)
```

## Comparing `autort-0.1.1.dist-info/LICENSE` & `autort-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

