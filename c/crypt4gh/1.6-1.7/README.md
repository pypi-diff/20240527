# Comparing `tmp/crypt4gh-1.6.tar.gz` & `tmp/crypt4gh-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypt4gh-1.6.tar", last modified: Wed Aug 10 10:46:20 2022, max compression
+gzip compressed data, was "crypt4gh-1.7.tar", last modified: Mon May 27 10:22:58 2024, max compression
```

## Comparing `crypt4gh-1.6.tar` & `crypt4gh-1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 daz        (501) staff       (20)        0 2022-08-10 10:46:20.713256 crypt4gh-1.6/
--rw-r--r--   0 daz        (501) staff       (20)    11357 2018-10-22 09:03:54.000000 crypt4gh-1.6/LICENSE
--rw-r--r--   0 daz        (501) staff       (20)     4292 2022-08-10 10:46:20.713155 crypt4gh-1.6/PKG-INFO
--rw-r--r--   0 daz        (501) staff       (20)     3135 2020-06-21 17:25:38.000000 crypt4gh-1.6/README.md
-drwxr-xr-x   0 daz        (501) staff       (20)        0 2022-08-10 10:46:20.710972 crypt4gh-1.6/crypt4gh/
--rw-r--r--   0 daz        (501) staff       (20)     2141 2022-08-10 10:36:15.000000 crypt4gh-1.6/crypt4gh/__init__.py
--rw-r--r--   0 daz        (501) staff       (20)      926 2020-03-11 20:00:52.000000 crypt4gh-1.6/crypt4gh/__main__.py
--rw-r--r--   0 daz        (501) staff       (20)     7544 2020-07-26 22:20:48.000000 crypt4gh-1.6/crypt4gh/cli.py
--rw-r--r--   0 daz        (501) staff       (20)     5082 2020-05-09 23:17:51.000000 crypt4gh-1.6/crypt4gh/debug.py
--rw-r--r--   0 daz        (501) staff       (20)     1328 2020-02-02 12:55:34.000000 crypt4gh-1.6/crypt4gh/exceptions.py
--rw-r--r--   0 daz        (501) staff       (20)    15422 2020-06-21 17:25:38.000000 crypt4gh-1.6/crypt4gh/header.py
-drwxr-xr-x   0 daz        (501) staff       (20)        0 2022-08-10 10:46:20.712916 crypt4gh-1.6/crypt4gh/keys/
--rw-r--r--   0 daz        (501) staff       (20)     6622 2021-03-07 12:32:06.000000 crypt4gh-1.6/crypt4gh/keys/__init__.py
--rw-r--r--   0 daz        (501) staff       (20)      224 2019-11-12 20:17:36.000000 crypt4gh-1.6/crypt4gh/keys/__main__.py
--rw-r--r--   0 daz        (501) staff       (20)     4714 2022-08-10 10:34:51.000000 crypt4gh-1.6/crypt4gh/keys/c4gh.py
--rw-r--r--   0 daz        (501) staff       (20)     2685 2019-11-13 17:13:37.000000 crypt4gh-1.6/crypt4gh/keys/debug.py
--rw-r--r--   0 daz        (501) staff       (20)     1629 2020-06-21 17:25:41.000000 crypt4gh-1.6/crypt4gh/keys/kdf.py
--rw-r--r--   0 daz        (501) staff       (20)     6958 2020-07-26 23:16:04.000000 crypt4gh-1.6/crypt4gh/keys/ssh.py
--rw-r--r--   0 daz        (501) staff       (20)    15621 2020-02-02 12:55:34.000000 crypt4gh-1.6/crypt4gh/lib.py
-drwxr-xr-x   0 daz        (501) staff       (20)        0 2022-08-10 10:46:20.711957 crypt4gh-1.6/crypt4gh.egg-info/
--rw-r--r--   0 daz        (501) staff       (20)     4292 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/PKG-INFO
--rw-r--r--   0 daz        (501) staff       (20)      524 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/SOURCES.txt
--rw-r--r--   0 daz        (501) staff       (20)        1 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/dependency_links.txt
--rw-r--r--   0 daz        (501) staff       (20)       98 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/entry_points.txt
--rw-r--r--   0 daz        (501) staff       (20)        1 2021-03-07 12:38:00.000000 crypt4gh-1.6/crypt4gh.egg-info/not-zip-safe
--rw-r--r--   0 daz        (501) staff       (20)       60 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/requires.txt
--rw-r--r--   0 daz        (501) staff       (20)        9 2022-08-10 10:46:20.000000 crypt4gh-1.6/crypt4gh.egg-info/top_level.txt
--rw-r--r--   0 daz        (501) staff       (20)       38 2022-08-10 10:46:20.713287 crypt4gh-1.6/setup.cfg
--rw-r--r--   0 daz        (501) staff       (20)     2195 2022-08-10 10:35:59.000000 crypt4gh-1.6/setup.py
+drwxr-xr-x   0 daz        (501) staff       (20)        0 2024-05-27 10:22:58.000797 crypt4gh-1.7/
+-rw-r--r--   0 daz        (501) staff       (20)    11357 2018-10-22 09:03:54.000000 crypt4gh-1.7/LICENSE
+-rw-r--r--   0 daz        (501) staff       (20)     4625 2024-05-27 10:22:58.000615 crypt4gh-1.7/PKG-INFO
+-rw-r--r--   0 daz        (501) staff       (20)     3333 2024-05-27 10:17:48.000000 crypt4gh-1.7/README.md
+drwxr-xr-x   0 daz        (501) staff       (20)        0 2024-05-27 10:22:57.998287 crypt4gh-1.7/crypt4gh/
+-rw-r--r--   0 daz        (501) staff       (20)     2141 2024-05-27 10:14:23.000000 crypt4gh-1.7/crypt4gh/__init__.py
+-rw-r--r--   0 daz        (501) staff       (20)      926 2023-07-22 14:20:41.000000 crypt4gh-1.7/crypt4gh/__main__.py
+-rw-r--r--   0 daz        (501) staff       (20)     8228 2024-05-27 10:14:23.000000 crypt4gh-1.7/crypt4gh/cli.py
+-rw-r--r--   0 daz        (501) staff       (20)     5082 2024-05-17 15:40:33.000000 crypt4gh-1.7/crypt4gh/debug.py
+-rw-r--r--   0 daz        (501) staff       (20)     1328 2020-02-02 12:55:34.000000 crypt4gh-1.7/crypt4gh/exceptions.py
+-rw-r--r--   0 daz        (501) staff       (20)    15422 2024-05-17 15:40:33.000000 crypt4gh-1.7/crypt4gh/header.py
+drwxr-xr-x   0 daz        (501) staff       (20)        0 2024-05-27 10:22:58.000103 crypt4gh-1.7/crypt4gh/keys/
+-rw-r--r--   0 daz        (501) staff       (20)     6622 2024-05-17 15:40:33.000000 crypt4gh-1.7/crypt4gh/keys/__init__.py
+-rw-r--r--   0 daz        (501) staff       (20)      224 2019-11-12 20:17:36.000000 crypt4gh-1.7/crypt4gh/keys/__main__.py
+-rw-r--r--   0 daz        (501) staff       (20)     4714 2022-08-10 10:34:51.000000 crypt4gh-1.7/crypt4gh/keys/c4gh.py
+-rw-r--r--   0 daz        (501) staff       (20)     2685 2019-11-13 17:13:37.000000 crypt4gh-1.7/crypt4gh/keys/debug.py
+-rw-r--r--   0 daz        (501) staff       (20)     1629 2020-06-21 17:25:41.000000 crypt4gh-1.7/crypt4gh/keys/kdf.py
+-rw-r--r--   0 daz        (501) staff       (20)     6958 2020-07-26 23:16:04.000000 crypt4gh-1.7/crypt4gh/keys/ssh.py
+-rw-r--r--   0 daz        (501) staff       (20)    15886 2024-05-27 10:14:23.000000 crypt4gh-1.7/crypt4gh/lib.py
+drwxr-xr-x   0 daz        (501) staff       (20)        0 2024-05-27 10:22:58.000409 crypt4gh-1.7/crypt4gh.egg-info/
+-rw-r--r--   0 daz        (501) staff       (20)     4625 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/PKG-INFO
+-rw-r--r--   0 daz        (501) staff       (20)      524 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/SOURCES.txt
+-rw-r--r--   0 daz        (501) staff       (20)        1 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/dependency_links.txt
+-rw-r--r--   0 daz        (501) staff       (20)       98 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/entry_points.txt
+-rw-r--r--   0 daz        (501) staff       (20)        1 2023-07-22 11:37:21.000000 crypt4gh-1.7/crypt4gh.egg-info/not-zip-safe
+-rw-r--r--   0 daz        (501) staff       (20)       60 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/requires.txt
+-rw-r--r--   0 daz        (501) staff       (20)        9 2024-05-27 10:22:57.000000 crypt4gh-1.7/crypt4gh.egg-info/top_level.txt
+-rw-r--r--   0 daz        (501) staff       (20)       38 2024-05-27 10:22:58.000835 crypt4gh-1.7/setup.cfg
+-rw-r--r--   0 daz        (501) staff       (20)     2195 2024-05-27 10:14:23.000000 crypt4gh-1.7/setup.py
```

### Comparing `crypt4gh-1.6/LICENSE` & `crypt4gh-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/PKG-INFO` & `crypt4gh-1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt4gh
-Version: 1.6
+Version: 1.7
 Summary: GA4GH cryptographic utilities
 Home-page: https://www.github.com/EGA-archive/crypt4gh
 Author: Frédéric Haziza
 Author-email: frederic.haziza@crg.eu
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,21 +22,26 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyYaml>=5.1.2
+Requires-Dist: docopt
+Requires-Dist: cryptography>=2.8
+Requires-Dist: pynacl>=1.3.0
+Requires-Dist: bcrypt
 
 [![Documentation Status](https://readthedocs.org/projects/crypt4gh/badge/?version=latest)](https://crypt4gh.readthedocs.io/en/latest/?badge=latest)
 [![Testsuite](https://github.com/EGA-archive/crypt4gh/workflows/Testsuite/badge.svg)](https://github.com/EGA-archive/crypt4gh/actions)
 
 # Crypt4GH Encryption Utility
 
-`crypt4gh`is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
+`crypt4gh` is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
 
 
 ## Installation
 
 Python `3.6+` required to use the crypt4gh encryption utility.
 
 Install it from PyPI:
@@ -65,29 +70,31 @@
 
 ```bash
 $ crypt4gh -h
 
 Utility for the cryptographic GA4GH standard, reading from stdin and outputting to stdout.
 
 Usage:
-   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]
+   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]  [--header <path>]
    {PROG} [-hv] [--log <file>] decrypt [--sk <path>] [--sender_pk <path>] [--range <start-end>]
    {PROG} [-hv] [--log <file>] rearrange [--sk <path>] --range <start-end>
-   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim]
+   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim] [--header-only]
 
 Options:
    -h, --help             Prints this help and exit
    -v, --version          Prints the version and exits
    --log <file>           Path to the logger file (in YML format)
    --sk <keyfile>         Curve25519-based Private key.
                           When encrypting, if neither the private key nor C4GH_SECRET_KEY are specified, we generate a new key 
    --recipient_pk <path>  Recipient's Curve25519-based Public key
    --sender_pk <path>     Peer's Curve25519-based Public key to verify provenance (akin to signature)
    --range <start-end>    Byte-range either as  <start-end> or just <start> (Start included, End excluded)
    -t, --trim             Keep only header packets that you can decrypt
+   --header <path>        Where to write the header (default: stdout)
+   --header-only          Whether the input data consists only of a header (default: false)
 
 
 Environment variables:
    C4GH_LOG         If defined, it will be used as the default logger
    C4GH_SECRET_KEY  If defined, it will be used as the default secret key (ie --sk ${C4GH_SECRET_KEY})
  
 ```
```

### Comparing `crypt4gh-1.6/README.md` & `crypt4gh-1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Documentation Status](https://readthedocs.org/projects/crypt4gh/badge/?version=latest)](https://crypt4gh.readthedocs.io/en/latest/?badge=latest)
 [![Testsuite](https://github.com/EGA-archive/crypt4gh/workflows/Testsuite/badge.svg)](https://github.com/EGA-archive/crypt4gh/actions)
 
 # Crypt4GH Encryption Utility
 
-`crypt4gh`is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
+`crypt4gh` is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
 
 
 ## Installation
 
 Python `3.6+` required to use the crypt4gh encryption utility.
 
 Install it from PyPI:
@@ -36,29 +36,31 @@
 
 ```bash
 $ crypt4gh -h
 
 Utility for the cryptographic GA4GH standard, reading from stdin and outputting to stdout.
 
 Usage:
-   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]
+   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]  [--header <path>]
    {PROG} [-hv] [--log <file>] decrypt [--sk <path>] [--sender_pk <path>] [--range <start-end>]
    {PROG} [-hv] [--log <file>] rearrange [--sk <path>] --range <start-end>
-   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim]
+   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim] [--header-only]
 
 Options:
    -h, --help             Prints this help and exit
    -v, --version          Prints the version and exits
    --log <file>           Path to the logger file (in YML format)
    --sk <keyfile>         Curve25519-based Private key.
                           When encrypting, if neither the private key nor C4GH_SECRET_KEY are specified, we generate a new key 
    --recipient_pk <path>  Recipient's Curve25519-based Public key
    --sender_pk <path>     Peer's Curve25519-based Public key to verify provenance (akin to signature)
    --range <start-end>    Byte-range either as  <start-end> or just <start> (Start included, End excluded)
    -t, --trim             Keep only header packets that you can decrypt
+   --header <path>        Where to write the header (default: stdout)
+   --header-only          Whether the input data consists only of a header (default: false)
 
 
 Environment variables:
    C4GH_LOG         If defined, it will be used as the default logger
    C4GH_SECRET_KEY  If defined, it will be used as the default secret key (ie --sk ${C4GH_SECRET_KEY})
  
 ```
```

### Comparing `crypt4gh-1.6/crypt4gh/__init__.py` & `crypt4gh-1.7/crypt4gh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #
 #
 # Finally, we do not yet implement slicing a file that already contains an Edit List
 #
 
 
 __title__ = 'GA4GH cryptographic utilities'
-__version__ = '1.6' # VERSION in header is 1 (as 4 bytes little endian)
+__version__ = '1.7' # VERSION in header is 1 (as 4 bytes little endian)
 __author__ = 'Frédéric Haziza'
 __author_email__ = 'frederic.haziza@crg.eu'
 __license__ = 'Apache License 2.0'
 __copyright__ = __title__ + ' @ CRG'
 
 PROG = 'crypt4gh'
```

### Comparing `crypt4gh-1.6/crypt4gh/__main__.py` & `crypt4gh-1.7/crypt4gh/__main__.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/cli.py` & `crypt4gh-1.7/crypt4gh/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,30 +22,31 @@
 DEFAULT_LOG = os.getenv('C4GH_LOG', None)
 
 __doc__ = f'''
 
 Utility for the cryptographic GA4GH standard, reading from stdin and outputting to stdout.
 
 Usage:
-   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]
+   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>] [--header <path>]
    {PROG} [-hv] [--log <file>] decrypt [--sk <path>] [--sender_pk <path>] [--range <start-end>]
    {PROG} [-hv] [--log <file>] rearrange [--sk <path>] --range <start-end>
-   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim]
+   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim] [--header-only]
 
 Options:
    -h, --help             Prints this help and exit
    -v, --version          Prints the version and exits
    --log <file>           Path to the logger file (in YML format)
    --sk <keyfile>         Curve25519-based Private key
                           When encrypting, if neither the private key nor C4GH_SECRET_KEY are specified, we generate a new key 
    --recipient_pk <path>  Recipient's Curve25519-based Public key
    --sender_pk <path>     Peer's Curve25519-based Public key to verify provenance (akin to signature)
    --range <start-end>    Byte-range either as  <start-end> or just <start> (Start included, End excluded)
    -t, --trim             Keep only header packets that you can decrypt
-
+   --header <path>        Where to write the header (default: stdout)
+   --header-only          Whether the input data consists only of a header (default: false)
 
 Environment variables:
    C4GH_LOG         If defined, it will be used as the default logger
    C4GH_SECRET_KEY  If defined, it will be used as the default secret key (ie --sk ${{C4GH_SECRET_KEY}})
    C4GH_PASSPHRASE  If defined, it will be used as the passphrase
                     for decoding the secret key, replacing the callback.
                     Note: this is insecure. Only used for testing
@@ -130,30 +131,40 @@
 
     seckey = retrieve_private_key(args, generate=True)
 
     def build_recipients():
         for pk in args['--recipient_pk']:
             recipient_pubkey = os.path.expanduser(pk)
             if not os.path.exists(recipient_pubkey):
+                print(f"Recipient pubkey: {recipient_pubkey}, does not exist", file=sys.stderr)
                 continue
             LOG.debug("Recipient pubkey: %s", recipient_pubkey)
             yield (0, seckey, get_public_key(recipient_pubkey))
 
     # keys = list of (method, privkey, recipient_pubkey=None)
     # using a set now, instead of inside the generator loop
     # because we'd remove repetition in case different filenames are used for the same key
     recipient_keys = set(build_recipients()) # must have at least one, remove repetitions
     if not recipient_keys:
         raise ValueError("No Recipients' Public Key found")
 
-    lib.encrypt(recipient_keys,
-                sys.stdin.buffer,
-                sys.stdout.buffer,
-                offset = range_start,
-                span = range_span)
+    header = args["--header"]
+
+    try:
+        if header:
+            header = open(header, 'wb') # let it raise exception
+        lib.encrypt(recipient_keys,
+                    sys.stdin.buffer,
+                    sys.stdout.buffer,
+                    headerfile = header,
+                    offset = range_start,
+                    span = range_span)
+    finally:
+        if header:
+            header.close()
     
 
 def decrypt(args):
     assert( args['decrypt'] )
 
     sender_pubkey = get_public_key(os.path.expanduser(args['--sender_pk'])) if args['--sender_pk'] else None
 
@@ -191,14 +202,15 @@
 
     seckey = retrieve_private_key(args)
 
     def build_recipients():
         for pk in args['--recipient_pk']:
             recipient_pubkey = os.path.expanduser(pk)
             if not os.path.exists(recipient_pubkey):
+                print(f"Recipient pubkey: {recipient_pubkey}, does not exist", file=sys.stderr)
                 continue
             LOG.debug("Recipient pubkey: %s", recipient_pubkey)
             yield (0, seckey, get_public_key(recipient_pubkey))
 
     # keys = list of (method, privkey, recipient_pubkey=None)
     # using a set now, instead of inside the generator loop
     # because we'd remove repetition in case different filenames are used for the same key
@@ -206,8 +218,9 @@
     if not recipient_keys:
         raise ValueError("No Recipients' Public Key found")
 
     lib.reencrypt([(0, seckey, None)], # sender_keys
                   recipient_keys,
                   sys.stdin.buffer,
                   sys.stdout.buffer,
-                  trim=args['--trim'])
+                  trim=args['--trim'],
+                  header_only=args['--header-only'])
```

### Comparing `crypt4gh-1.6/crypt4gh/debug.py` & `crypt4gh-1.7/crypt4gh/debug.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/exceptions.py` & `crypt4gh-1.7/crypt4gh/exceptions.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/header.py` & `crypt4gh-1.7/crypt4gh/header.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/keys/__init__.py` & `crypt4gh-1.7/crypt4gh/keys/__init__.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/keys/c4gh.py` & `crypt4gh-1.7/crypt4gh/keys/c4gh.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/keys/debug.py` & `crypt4gh-1.7/crypt4gh/keys/debug.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/keys/kdf.py` & `crypt4gh-1.7/crypt4gh/keys/kdf.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/keys/ssh.py` & `crypt4gh-1.7/crypt4gh/keys/ssh.py`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/crypt4gh/lib.py` & `crypt4gh-1.7/crypt4gh/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,25 +42,27 @@
     nonce = os.urandom(12)
     encrypted_data = crypto_aead_chacha20poly1305_ietf_encrypt(data, None, nonce, key)  # no add
     process(nonce) # after producing the segment, so we don't start outputing when an error occurs
     process(encrypted_data)
 
 
 @close_on_broken_pipe
-def encrypt(keys, infile, outfile, offset=0, span=None):
+def encrypt(keys, infile, outfile, headerfile=None, offset=0, span=None):
     '''Encrypt infile into outfile, using the list of keys.
 
 
     It fast-forwards to `offset` and encrypts until
     a total of `span` bytes is reached (or to EOF if `span` is None)
 
     This produces a Crypt4GH file without edit list.
     '''
 
     LOG.info('Encrypting the file')
+    
+    headerfile = headerfile or outfile
 
     # Forward to start position
     LOG.debug("  Start Coordinate: %s", offset)
     try:
         offset = int(offset)
         if offset < 0:
             offset = 0
@@ -87,15 +89,15 @@
     # Output the header
     LOG.debug('Creating Crypt4GH header')
     header_content = header.make_packet_data_enc(encryption_method, session_key)
     header_packets = header.encrypt(header_content, keys)
     header_bytes = header.serialize(header_packets)
 
     LOG.debug('header length: %d', len(header_bytes))
-    outfile.write(header_bytes)
+    headerfile.write(header_bytes)
 
     # ...and cue music
     LOG.debug("Streaming content")
     # oh boy... I buffer a whole segment!
     # TODO: Use a smaller buffer (Requires code rewrite)
     segment = bytearray(SEGMENT_SIZE)
 
@@ -282,14 +284,17 @@
         segment = decrypt_block(data, self.session_keys)
         LOG.debug('Adding %d bytes to the buffer', len(segment))
         self._append_to_buf(segment)
         LOG.debug('Buffer size: %d', self.buf_size())
         
     def skip(self, size):
         """Skip size bytes."""
+        if not size:
+            return
+
         assert(size > 0)
         LOG.debug('Skipping %d bytes | Buffer size: %d', size, self.buf_size())
 
         while size > 0:
             # Empty the buffer
             LOG.debug('Left to skip: %d | Buffer size: %d', size, self.buf_size())
             b = self.buf.read(size)
@@ -398,23 +403,28 @@
 ##
 ##    Just reencryption of the header
 ##
 ##############################################################
 
 
 @close_on_broken_pipe
-def reencrypt(keys, recipient_keys, infile, outfile, chunk_size=4096, trim=False):
+def reencrypt(keys, recipient_keys, infile, outfile, chunk_size=4096, trim=False, header_only=False):
     '''Extract header packets from infile and generate another one to outfile.
     The encrypted data section is only copied from infile to outfile.'''
 
     # Decrypt and re-encrypt the header
     header_packets = header.parse(infile)
     packets = header.reencrypt(header_packets, keys, recipient_keys, trim=trim)
     outfile.write(header.serialize(packets))
 
+    # If header-only reencryption, we are done.
+    if header_only:
+        LOG.info(f'Header-only reencryption Successful')
+        return
+
     # Stream the remainder
     LOG.info(f'Streaming the remainder of the file')
     while True:
         data = infile.read(chunk_size)
         if not data:
             break
         outfile.write(data)
```

### Comparing `crypt4gh-1.6/crypt4gh.egg-info/PKG-INFO` & `crypt4gh-1.7/crypt4gh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt4gh
-Version: 1.6
+Version: 1.7
 Summary: GA4GH cryptographic utilities
 Home-page: https://www.github.com/EGA-archive/crypt4gh
 Author: Frédéric Haziza
 Author-email: frederic.haziza@crg.eu
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,21 +22,26 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyYaml>=5.1.2
+Requires-Dist: docopt
+Requires-Dist: cryptography>=2.8
+Requires-Dist: pynacl>=1.3.0
+Requires-Dist: bcrypt
 
 [![Documentation Status](https://readthedocs.org/projects/crypt4gh/badge/?version=latest)](https://crypt4gh.readthedocs.io/en/latest/?badge=latest)
 [![Testsuite](https://github.com/EGA-archive/crypt4gh/workflows/Testsuite/badge.svg)](https://github.com/EGA-archive/crypt4gh/actions)
 
 # Crypt4GH Encryption Utility
 
-`crypt4gh`is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
+`crypt4gh` is a Python tool to encrypt, decrypt or re-encrypt files, according to the [GA4GH encryption file format](https://www.ga4gh.org/news/crypt4gh-a-secure-method-for-sharing-human-genetic-data/).
 
 
 ## Installation
 
 Python `3.6+` required to use the crypt4gh encryption utility.
 
 Install it from PyPI:
@@ -65,29 +70,31 @@
 
 ```bash
 $ crypt4gh -h
 
 Utility for the cryptographic GA4GH standard, reading from stdin and outputting to stdout.
 
 Usage:
-   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]
+   {PROG} [-hv] [--log <file>] encrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--range <start-end>]  [--header <path>]
    {PROG} [-hv] [--log <file>] decrypt [--sk <path>] [--sender_pk <path>] [--range <start-end>]
    {PROG} [-hv] [--log <file>] rearrange [--sk <path>] --range <start-end>
-   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim]
+   {PROG} [-hv] [--log <file>] reencrypt [--sk <path>] --recipient_pk <path> [--recipient_pk <path>]... [--trim] [--header-only]
 
 Options:
    -h, --help             Prints this help and exit
    -v, --version          Prints the version and exits
    --log <file>           Path to the logger file (in YML format)
    --sk <keyfile>         Curve25519-based Private key.
                           When encrypting, if neither the private key nor C4GH_SECRET_KEY are specified, we generate a new key 
    --recipient_pk <path>  Recipient's Curve25519-based Public key
    --sender_pk <path>     Peer's Curve25519-based Public key to verify provenance (akin to signature)
    --range <start-end>    Byte-range either as  <start-end> or just <start> (Start included, End excluded)
    -t, --trim             Keep only header packets that you can decrypt
+   --header <path>        Where to write the header (default: stdout)
+   --header-only          Whether the input data consists only of a header (default: false)
 
 
 Environment variables:
    C4GH_LOG         If defined, it will be used as the default logger
    C4GH_SECRET_KEY  If defined, it will be used as the default secret key (ie --sk ${C4GH_SECRET_KEY})
  
 ```
```

### Comparing `crypt4gh-1.6/crypt4gh.egg-info/SOURCES.txt` & `crypt4gh-1.7/crypt4gh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypt4gh-1.6/setup.py` & `crypt4gh-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 from setuptools import setup, find_packages
 
 _readme = (Path(__file__).parent / "README.md").read_text()
 
 setup(name='crypt4gh',
-      version='1.6',
+      version='1.7',
       url='https://www.github.com/EGA-archive/crypt4gh',
       license='Apache License 2.0',
       author='Frédéric Haziza',
       author_email='frederic.haziza@crg.eu',
       description='GA4GH cryptographic utilities',
       long_description=_readme,
       long_description_content_type="text/markdown",
```

