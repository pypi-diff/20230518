# Comparing `tmp/pycvc-1.2.5.tar.gz` & `tmp/pycvc-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycvc-1.2.5.tar", last modified: Wed May 17 07:18:35 2023, max compression
+gzip compressed data, was "pycvc-1.2.6.tar", last modified: Thu May 18 08:14:48 2023, max compression
```

## Comparing `pycvc-1.2.5.tar` & `pycvc-1.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:18:35.567591 pycvc-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-17 07:18:35.567591 pycvc-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-05-17 07:18:22.000000 pycvc-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:18:35.567591 pycvc-1.2.5/cvc/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/ec_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:18:35.567591 pycvc-1.2.5/cvc/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12963 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/tools/cvc_create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4829 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/tools/cvc_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-17 07:18:22.000000 pycvc-1.2.5/cvc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:18:35.567591 pycvc-1.2.5/pycvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-17 07:18:35.000000 pycvc-1.2.5/pycvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:18:35.567591 pycvc-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 07:18:22.000000 pycvc-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:14:48.020572 pycvc-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-18 08:14:48.020572 pycvc-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-18 08:14:36.000000 pycvc-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:14:48.016572 pycvc-1.2.6/cvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/ec_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:14:48.016572 pycvc-1.2.6/cvc/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13130 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/tools/cvc_create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4829 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/tools/cvc_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-18 08:14:36.000000 pycvc-1.2.6/cvc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:14:48.020572 pycvc-1.2.6/pycvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 08:14:48.000000 pycvc-1.2.6/pycvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 08:14:48.020572 pycvc-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-18 08:14:36.000000 pycvc-1.2.6/setup.py
```

### Comparing `pycvc-1.2.5/PKG-INFO` & `pycvc-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycvc
-Version: 1.2.5
+Version: 1.2.6
 Summary: Card Verifiable Certificate tools
 Home-page: https://github.com/polhenarejos/pycvc
 Author: Pol Henarejos
 Author-email: pol.henarejos@cttc.es
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -58,66 +58,66 @@
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl ecparam -out ZZATCVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl ecparam -out ZZATDVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl ec -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Create a PKI with RSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl genrsa -out ZZATCVCA00001.pem 3072
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl genrsa -out ZZATDVCA00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl rsa -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl genrsa -out ZZATTERM00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=RSA_v1_5_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Validate certificates and requests
 
 `cvc-print` is the tool for certificate validation and verification. Call `cvc-print --help` for a complete list of parameters.
 
 The validation is performed by veryfing all signatures in the certificate chain.
```

### Comparing `pycvc-1.2.5/README.md` & `pycvc-1.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,66 +29,66 @@
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl ecparam -out ZZATCVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl ecparam -out ZZATDVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl ec -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Create a PKI with RSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl genrsa -out ZZATCVCA00001.pem 3072
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl genrsa -out ZZATDVCA00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl rsa -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl genrsa -out ZZATTERM00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=RSA_v1_5_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Validate certificates and requests
 
 `cvc-print` is the tool for certificate validation and verification. Call `cvc-print --help` for a complete list of parameters.
 
 The validation is performed by veryfing all signatures in the certificate chain.
```

### Comparing `pycvc-1.2.5/cvc/_version.py` & `pycvc-1.2.6/cvc/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
  * General Public License for more details.
  *
  * You should have received a copy of the GNU General Public License
  * along with this program. If not, see <http://www.gnu.org/licenses/>.
  */
 """
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
```

### Comparing `pycvc-1.2.5/cvc/asn1.py` & `pycvc-1.2.6/cvc/asn1.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/cvc/certificates.py` & `pycvc-1.2.6/cvc/certificates.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,18 @@
         self.__a = ASN1()
 
     def decode(self, data):
         self.__data = data
         self.__a = ASN1().decode(self.__data)
         return self
 
-    def body(self, pubkey=None, scheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
+    def body(self, pubkey=None, scheme=None, car=None, chr=None, role=None, days=None, since=None, extensions=None, req=False):
         if (self.__data != None):
             return self.cert().find(0x7f4e)
-        self.__a = ASN1().add_tag(0x7f4e, self.cpi().car(car).pubkey(pubkey, scheme, req).chr(chr).role(role).valid(valid, since).extensions(extensions).encode())
+        self.__a = ASN1().add_tag(0x7f4e, self.cpi().car(car).pubkey(pubkey, scheme, req).chr(chr).role(role).valid(days=days, since=since).extensions(extensions).encode())
         return self
 
     def extensions(self, extensions=None):
         if (self.__data != None):
             return self.body().find(0x65)
         if (extensions != None):
             data = b''
@@ -95,21 +95,21 @@
     def role(self, role=None):
         if (self.__data != None):
             return self.body().find(0x7f4c)
         if (role != None):
             self.__a = self.__a.add_tag(0x7f4c, ASN1().add_oid(role.OID).add_tag(0x53, role.to_bytes()).encode())
         return self
 
-    def valid(self, valid=None, since=None):
+    def valid(self, days=None, since=None):
         if (self.__data != None):
             return self.body().find(0x5f25).data()
-        if (valid != None):
-            if (since == None):
+        if (days):
+            if (not since):
                 since = datetime.datetime.now().strftime("%y%m%d")
-            until = (datetime.datetime.strptime(since, "%y%m%d") + datetime.timedelta(days = int(valid))).strftime("%y%m%d")
+            until = (datetime.datetime.strptime(since, "%y%m%d") + datetime.timedelta(days = int(days))).strftime("%y%m%d")
             self.__a = self.__a.add_tag(0x5f25, bcd(since)).add_tag(0x5f24, bcd(until))
         return self
 
     def expires(self):
         return self.body().find(0x5f24).data()
 
     def signature(self):
@@ -127,27 +127,27 @@
             r,s = utils.decode_dss_signature(signature)
             signature = to_bytes(r) + to_bytes(s)
         elif (isinstance(key, rsa.RSAPrivateKey)):
             signature = key.sign(self.__a.encode(), p, h)
         self.__a = self.__a.add_tag(0x5f37, bytearray(signature))
         return self
 
-    def cert(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, role=None, valid=None, since=None, extensions=None, req=False):
+    def cert(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, role=None, days=None, since=None, extensions=None, req=False):
         if (self.__data != None):
             return self.req().find(0x7f21)
-        self.__a = ASN1().add_tag(0x7f21, self.body(pubkey, scheme, car, chr, role, valid, since, extensions, req or chr==car).sign(signkey, signscheme).encode())
+        self.__a = ASN1().add_tag(0x7f21, self.body(pubkey, scheme, car, chr, role, days, since, extensions, req or chr==car).sign(signkey, signscheme).encode())
         return self
 
     def req(self, pubkey=None, scheme=None, signkey=None, signscheme=None, car=None, chr=None, outercar=None, outerkey=None, outerscheme=None, extensions=None):
         if (self.__data != None):
             aut = ASN1().decode(self.__data).find(0x67)
             if (aut):
                 return aut
             return ASN1().decode(self.__data)
-        cert = self.cert(pubkey, scheme, signkey, signscheme, car, chr, role=None, valid=None, since=None, extensions=extensions, req=True)
+        cert = self.cert(pubkey, scheme, signkey, signscheme, car, chr, role=None, days=None, since=None, extensions=extensions, req=True)
         if (outercar != None and outerkey != None and outerscheme != None):
             self.__a = ASN1().add_tag(0x67, cert.car(outercar).sign(outerkey, outerscheme).encode())
         return self
 
     def is_req(self):
         if (self.__data != None):
             b = self.__a
```

### Comparing `pycvc-1.2.5/cvc/ec_curves.py` & `pycvc-1.2.6/cvc/ec_curves.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/cvc/oid.py` & `pycvc-1.2.6/cvc/oid.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/cvc/terminal.py` & `pycvc-1.2.6/cvc/terminal.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/cvc/tools/cvc_create.py` & `pycvc-1.2.6/cvc/tools/cvc_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Generate a Card Verifiable Certificate')
     parser.add_argument('--version', help='Displays the current version', action='store_true')
     parser.add_argument('-o','--out-cert', help='Generated certificate file', metavar='FILENAME')
     parser.add_argument('-r','--role', help='The role of entity', choices=['cvca','dv_domestic','dv_foreign','terminal'])
     parser.add_argument('-t','--type', help='The type of terminal. If not provided, it creates a certificate request', choices=['at','is','st'])
-    parser.add_argument('--valid', help='Days of validity since today or date provided by --since', default=90)
+    parser.add_argument('--days', help='Days of validity since today (or since --since)', default=90)
+    parser.add_argument('--since', help='Certificate effective date (use with caution) [in YYMMDD format]', metavar='YYMMDD')
     parser.add_argument('-k','--sign-key', help='Private key to sign the certificate.', required=True, metavar='FILENAME')
     parser.add_argument('--sign-as', help='CV certificate of signing entity. If not provided, the certificate is self-signed [generates a certificate]', metavar='FILENAME')
     parser.add_argument('--outer-as', help='Outer certificate for CV request', metavar='FILENAME')
     parser.add_argument('--outer-key', help='Private key for outer signature of CV request', metavar='FILENAME')
     parser.add_argument('-p','--public-key', help='The public key contained in the certificate. If not provided, it is derived from the sign-key', metavar='FILENAME')
     parser.add_argument('-q','--request', help='Generates a certificate based on a request', metavar='FILENAME')
     parser.add_argument('--out-key', help='File to store the generated private key [default CHR.pkcs8]', metavar='FILENAME')
@@ -191,15 +192,16 @@
         else:
             pub_key = sign_key.public_key()
 
     role = get_role(args.role)
 
     typ = get_type(args.type, role, args)
 
-    typ.chat(args.chat)
+    if (typ):
+        typ.chat(args.chat)
 
     if (not puboid):
         puboid = oid.scheme2oid(args.scheme)
     if (not puboid):
         if (isinstance(pub_key, rsa.RSAPublicKey)):
             puboid = oid.ID_TA_RSA_PSS_SHA256
         elif (isinstance(pub_key, ec.EllipticCurvePublicKey)):
@@ -221,15 +223,15 @@
             outercar, outerscheme = parse_as(args.outer_as)
             outerkey = load_private_key(args.outer_key)
         else:
             outercar,outerscheme,outerkey = None,None,None
         cert = CVC().req(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, outercar=outercar, outerkey=outerkey, outerscheme=outerscheme)
         ext = 'cvreq'
     else:
-        cert = CVC().cert(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, role=typ, valid=args.valid if typ else None)
+        cert = CVC().cert(pub_key, puboid, sign_key, signscheme, car=car, chr=chr, role=typ, days=args.days if typ else None, since=args.since if typ else None)
         ext = 'cvcert'
 
     with open(args.out_cert if args.out_cert != None else chr.decode()+'.'+ext,'wb') as f:
         f.write(cert.encode())
 
 def run():
     args = parse_args()
```

### Comparing `pycvc-1.2.5/cvc/tools/cvc_print.py` & `pycvc-1.2.6/cvc/tools/cvc_print.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/cvc/utils.py` & `pycvc-1.2.6/cvc/utils.py`

 * *Files identical despite different names*

### Comparing `pycvc-1.2.5/pycvc.egg-info/PKG-INFO` & `pycvc-1.2.6/pycvc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycvc
-Version: 1.2.5
+Version: 1.2.6
 Summary: Card Verifiable Certificate tools
 Home-page: https://github.com/polhenarejos/pycvc
 Author: Pol Henarejos
 Author-email: pol.henarejos@cttc.es
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -58,66 +58,66 @@
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl ecparam -out ZZATCVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl ecparam -out ZZATDVCA00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl ec -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=ECDSA_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl ecparam -out ZZATTERM00001.pem -name prime256v1 -genkey
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=ECDSA_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Create a PKI with RSA
 
 `cvc-create` is the tool to create certificates or requests. Call `cvc-create --help` for a complete list of parameters.
 
 1- Setup the CA:
 ```bash
 openssl genrsa -out ZZATCVCA00001.pem 3072
 openssl pkcs8 -topk8 -nocrypt -in ZZATCVCA00001.pem -outform DER -out ZZATCVCA00001.pkcs8
-cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --valid=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
+cvc-create --role=cvca --type=at --chr=ZZATCVCA00001 --days=365 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256
 ```
 
 2- Setup the DV:
 ```bash
 openssl genrsa -out ZZATDVCA00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATDVCA00001.pem -outform DER -out ZZATDVCA00001.pkcs8
 openssl rsa -in ZZATDVCA00001.pem -out ZZATDVCA00001.pub -pubout -outform DER
-cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --valid=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
+cvc-create --role=dv_domestic --type=at --chr=ZZATDVCA00001 --days=180 --sign-key=ZZATCVCA00001.pkcs8 --scheme=RSA_v1_5_SHA_256 --sign-as=ZZATCVCA00001.cvcert --public-key=ZZATDVCA00001.pub
 ```
 
 3- Create a certificate request
 ```bash
 openssl genrsa -out ZZATTERM00001.pem 2048
 openssl pkcs8 -topk8 -nocrypt -in ZZATTERM00001.pem -outform DER -out ZZATTERM00001.pkcs8
 cvc-create --chr=ZZATTERM00001 --scheme=RSA_v1_5_SHA_256 --sign-key=ZZATTERM00001.pkcs8 --out-cert=ZZATTERM00001.cvreq --req-car=ZZATDVCA00001
 ```
 
 4- Sign a certificate request
 ```bash
-cvc-create --role=terminal --type=at --valid=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
+cvc-create --role=terminal --type=at --days=60 --sign-key=ZZATDVCA00001.pkcs8 --sign-as=ZZATDVCA00001.cvcert --request=ZZATTERM00001.cvreq
 ```
 
 ### Validate certificates and requests
 
 `cvc-print` is the tool for certificate validation and verification. Call `cvc-print --help` for a complete list of parameters.
 
 The validation is performed by veryfing all signatures in the certificate chain.
```

### Comparing `pycvc-1.2.5/setup.py` & `pycvc-1.2.6/setup.py`

 * *Files identical despite different names*

