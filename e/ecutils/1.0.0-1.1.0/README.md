# Comparing `tmp/ecutils-1.0.0.tar.gz` & `tmp/ecutils-1.1.0.tar.gz`

## Comparing `ecutils-1.0.0.tar` & `ecutils-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ecutils-1.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ecutils-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 ecutils-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 ecutils-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 ecutils-1.0.0/SECURITY.md
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 ecutils-1.0.0/mkdocs.yml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ecutils-1.0.0/requirements-docs.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ecutils-1.0.0/requirements-tests.txt
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ecutils-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ecutils-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 ecutils-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/index.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/installation.md
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/usage.md
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/algorithms/digital_signature.md
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/algorithms/koblitz.md
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/core/elliptic_curve.md
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/core/point.md
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/protocols/diffie_hellman.md
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/protocols/massey_omura.md
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ecutils-1.0.0/docs/reference/curves.md
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 ecutils-1.0.0/src/ecutils/__init__.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 ecutils-1.0.0/src/ecutils/algorithms.py
--rwxr-xr-x   0        0        0     4100 2020-02-02 00:00:00.000000 ecutils-1.0.0/src/ecutils/core.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 ecutils-1.0.0/src/ecutils/curves.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 ecutils-1.0.0/src/ecutils/protocols.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_diffie_hellman.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_digital_signature.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_elliptic_curve_operations.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_get_curve.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_koblitz.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ecutils-1.0.0/tests/test_massey_omura.py
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 ecutils-1.0.0/.gitignore
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 ecutils-1.0.0/LICENSE.md
--rwxr-xr-x   0        0        0     3996 2020-02-02 00:00:00.000000 ecutils-1.0.0/README.md
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 ecutils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 ecutils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ecutils-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ecutils-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 ecutils-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 ecutils-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ecutils-1.1.0/SECURITY.md
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 ecutils-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 ecutils-1.1.0/requirements-docs.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ecutils-1.1.0/requirements-tests.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ecutils-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ecutils-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 ecutils-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/index.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/installation.md
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/usage.md
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/algorithms/digital_signature.md
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/algorithms/koblitz.md
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/core/elliptic_curve.md
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/core/point.md
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/protocols/diffie_hellman.md
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/protocols/massey_omura.md
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 ecutils-1.1.0/docs/reference/curves.md
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/__init__.py
+-rw-r--r--   0        0        0    13893 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/algorithms.py
+-rwxr-xr-x   0        0        0     9443 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/core.py
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/curves.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/protocols.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 ecutils-1.1.0/src/ecutils/utils.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_diffie_hellman.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_digital_signature.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_elliptic_curve_operations.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_get_curve.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_koblitz.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 ecutils-1.1.0/tests/test_massey_omura.py
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 ecutils-1.1.0/.gitignore
+-rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 ecutils-1.1.0/LICENSE.md
+-rwxr-xr-x   0        0        0     6132 2020-02-02 00:00:00.000000 ecutils-1.1.0/README.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 ecutils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 ecutils-1.1.0/PKG-INFO
```

### Comparing `ecutils-1.0.0/CHANGELOG.md` & `ecutils-1.1.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.1.0] - 2024-04-22
+
+### Added
+- Added operations in Jacobian coordinates to improve calculation efficiency.
+
+### Changed
+- Updated version to v1.1.0, making it the official stable version.
+
+## [v1.0.0] - 2024-04-22
+
+### Added
+- Updated code of conduct and security policy.
+
+### Changed
+- Updated version to v1.0.0, making it the official stable version.
+
 ## [v0.0.1] - 2024-04-05
 
 ### Added
 - Added names of new authors to the project.
 
 ### Changed
 - Updated version to v0.0.1, making it the official stable version.
@@ -26,8 +42,8 @@
 ### Removed
 - Features, classes, or methods from version 0.0.1.dev4 that were not applicable to the redesigned architecture.
 
 ### Fixed
 - Issues and bugs that were present in the previous version have been addressed.
 
 ### Deprecated
-- Support for version 0.0.1.dev4 has been discontinued due to the significant changes in the project.
+- Support for version 0.0.1.dev4 has been discontinued due to the significant changes in the project.
```

### Comparing `ecutils-1.0.0/CODE_OF_CONDUCT.md` & `ecutils-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/CONTRIBUTING.md` & `ecutils-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/SECURITY.md` & `ecutils-1.1.0/SECURITY.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Supported Versions
 
 Use this section to tell people about which versions of your project are currently being supported with security updates.
 
 | Version | Supported          |
 | ------- | ------------------ |
+| 1.1.0   | :white_check_mark: |
 | 1.0.0   | :white_check_mark: |
 | 0.0.1   | :x:                |
 | 0.0.1a0   | :x:                |
 | 0.0.1.dev4   | :x:                |
 | 0.0.1.dev3   | :x:                |
 | 0.0.1.dev2   | :x:                |
 | 0.0.1.dev1   | :x:                |
```

### Comparing `ecutils-1.0.0/mkdocs.yml` & `ecutils-1.1.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Project information
 site_name: ECUtils
-site_url: https://ecutils.readthedocs.io/en/latest/
+site_url: https://ecutils.readthedocs.io/en/stable/
 site_author: Isak Ruas
 site_description: >-
   A comprehensive Python library for elliptic curve operations, providing utilities
   for common tasks such as digital signature generation and verification (ECDSA),
   key exchange protocols (ECDH and Massey-Omura), message encoding onto elliptic
   curves (Koblitz) as well as various elliptic curve operations. It is designed to be
   easy-to-use for cryptographic purposes and to facilitate the harnessing of
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # Project information site_name: ECUtils site_url: https://
-ecutils.readthedocs.io/en/latest/ site_author: Isak Ruas site_description: >- A
+ecutils.readthedocs.io/en/stable/ site_author: Isak Ruas site_description: >- A
 comprehensive Python library for elliptic curve operations, providing utilities
 for common tasks such as digital signature generation and verification (ECDSA),
 key exchange protocols (ECDH and Massey-Omura), message encoding onto elliptic
 curves (Koblitz) as well as various elliptic curve operations. It is designed
 to be easy-to-use for cryptographic purposes and to facilitate the harnessing
 of elliptic curve cryptography for security applications. # Repository
 repo_name: isakruas/ecutils repo_url: https://github.com/isakruas/ecutils #
```

### Comparing `ecutils-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ecutils-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `ecutils-1.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/.github/workflows/ci.yml` & `ecutils-1.1.0/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: '3.8'
+          python-version: '3.9'
 
       - name: Install dependencies
         run: |
           pip install -e .
           pip install -r requirements-tests.txt
           pip install pytest pytest-cov
```

### Comparing `ecutils-1.0.0/docs/index.md` & `ecutils-1.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/installation.md` & `ecutils-1.1.0/docs/installation.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 ```python
 from ecutils.algorithms import DigitalSignature
 
 # The rest of your code goes here
 ```
 
-Need more guidance? Check out our [documentation](https://ecutils.readthedocs.io/en/latest/).
+Need more guidance? Check out our [documentation](https://ecutils.readthedocs.io/en/stable/).
 
 Keep in mind to stay updated; run this every now and then:
 
 ```bash
 pip install --upgrade ecutils
 ```
```

### Comparing `ecutils-1.0.0/docs/usage.md` & `ecutils-1.1.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/algorithms/digital_signature.md` & `ecutils-1.1.0/docs/algorithms/digital_signature.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/algorithms/koblitz.md` & `ecutils-1.1.0/docs/algorithms/koblitz.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/core/elliptic_curve.md` & `ecutils-1.1.0/docs/core/elliptic_curve.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/core/point.md` & `ecutils-1.1.0/docs/core/point.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/protocols/diffie_hellman.md` & `ecutils-1.1.0/docs/protocols/diffie_hellman.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/protocols/massey_omura.md` & `ecutils-1.1.0/docs/protocols/massey_omura.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/docs/reference/curves.md` & `ecutils-1.1.0/docs/reference/curves.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/src/ecutils/curves.py` & `ecutils-1.1.0/src/ecutils/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import lru_cache
+
 from ecutils.core import EllipticCurve, Point
 
 secp192k1 = EllipticCurve(
     p=0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEFFFFEE37,
     a=0x0,
     b=0x3,
     G=Point(
@@ -95,14 +97,15 @@
         y=0x11839296A789A3BC0045C8A5FB42C7D1BD998F54449579B446817AFBD17273E662C97EE72995EF42640C550B9013FAD0761353C7086A272C24088BE94769FD16650,
     ),
     n=0x1FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFA51868783BF2F966B7FCC0148F709A5D03BB5C9B8899C47AEBB6FB71E91386409,
     h=0x1,
 )
 
 
+@lru_cache(maxsize=1024, typed=True)
 def get(name) -> EllipticCurve:
     """Retrieve an EllipticCurve instance by its standard name.
 
     Args:
         name (str): The standard name of the elliptic curve to retrieve.
                     Should be one of 'secp192k1', 'secp192r1', 'secp224k1',
                     'secp224r1', 'secp256k1', 'secp256r1', 'secp384r1', or 'secp521r1'.
```

### Comparing `ecutils-1.0.0/tests/test_diffie_hellman.py` & `ecutils-1.1.0/tests/test_diffie_hellman.py`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/tests/test_digital_signature.py` & `ecutils-1.1.0/tests/test_digital_signature.py`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/tests/test_elliptic_curve_operations.py` & `ecutils-1.1.0/tests/test_elliptic_curve_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,24 @@
             calculated_sum,
             self.point1,
             "Adding the identity element should return the original point.",
         )
 
     def test_invalid_scalar_multiplication(self):
         """Test scalar multiplication with invalid scalar or point."""
-        with self.assertRaises(ValueError):
+        with self.assertRaises(ValueError, msg="Test multiplying by scalar 0"):
             self.curve.multiply_point(0, self.point1)  # Test multiplying by scalar 0
-        with self.assertRaises(ValueError):
+        with self.assertRaises(
+            ValueError, msg="Test multiplying by scalar n (or larger)"
+        ):
             self.curve.multiply_point(
                 self.curve.n, self.point1
             )  # Test multiplying by scalar n (or larger)
         off_curve_point = Point(x=200, y=119)
-        with self.assertRaises(ValueError):
+        with self.assertRaises(ValueError, msg="Test with point not on the curve"):
             self.curve.multiply_point(
                 2, off_curve_point
             )  # Test with point not on the curve
 
     def test_addition_of_inverses_leading_to_infinity(self):
         """Test adding a point on the curve to its inverse, which should lead to
         the point at infinity."""
```

### Comparing `ecutils-1.0.0/tests/test_get_curve.py` & `ecutils-1.1.0/tests/test_get_curve.py`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/tests/test_koblitz.py` & `ecutils-1.1.0/tests/test_koblitz.py`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/tests/test_massey_omura.py` & `ecutils-1.1.0/tests/test_massey_omura.py`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/LICENSE.md` & `ecutils-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecutils-1.0.0/README.md` & `ecutils-1.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Elliptic Curve Utils (ecutils)
-[![Documentation Status](https://readthedocs.org/projects/ecutils/badge/?version=latest)](https://ecutils.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/ecutils/badge/?version=latest)](https://ecutils.readthedocs.io/en/stable/?badge=latest)
 [![Latest Version](https://img.shields.io/pypi/v/ecutils.svg?style=flat)](https://pypi.python.org/pypi/ecutils/)
 [![Downloads](https://static.pepy.tech/badge/ecutils)](https://pepy.tech/project/ecutils)
 [![Downloads](https://static.pepy.tech/badge/ecutils/month)](https://pepy.tech/project/ecutils)
 [![Downloads](https://static.pepy.tech/badge/ecutils/week)](https://pepy.tech/project/ecutils)
 [![codecov](https://codecov.io/gh/isakruas/ecutils/branch/master/graph/badge.svg)](https://codecov.io/gh/isakruas/ecutils)
 
 Elliptic Curve Utils, or `ecutils`, is a Python package that provides utilities for working with elliptic curves, particularly in the context of cryptography. It includes functionality for operations like point addition and scalar multiplication on curves, as well as higher-level protocols like key exchange and digital signatures.
@@ -75,17 +75,78 @@
 
 # Bob computes his shared secret with Alice's public key
 bob_shared_secret = bob.compute_shared_secret(alice.public_key)
 
 # alice_shared_secret should be equal to bob_shared_secret
 ```
 
+### Massey-Omura Key Exchange
+
+```python
+from ecutils.protocols import MasseyOmura
+from ecutils.algorithms import Koblitz
+
+# Initialize the Koblitz instance for the elliptic curve 'secp192k1'
+koblitz = Koblitz(curve_name='secp192k1')
+
+# Sender's side
+# -------------
+# Sender chooses their private key
+private_key_sender = 123456789
+# Initialize Massey-Omura protocol with the sender's private key
+mo_sender = MasseyOmura(private_key_sender, curve_name='secp192k1')
+
+# Encode the message using the Koblitz method
+# `j` is used to handle the ambiguity in the decoding process
+message, j = koblitz.encode("Hello, world!")
+
+# Perform the first encryption step with Massey-Omura protocol
+encrypted_msg_sender = mo_sender.first_encryption_step(message)
+
+# The encoded message is now sent to the receiver...
+# (transmission of encrypted_msg_sender)
+
+# Receiver's side
+# ---------------
+# Receiver chooses their private key
+private_key_receiver = 987654321
+# Initialize Massey-Omura protocol with the receiver's private key
+mo_receiver = MasseyOmura(private_key_receiver, curve_name='secp192k1')
+
+# Perform the second encryption step with Massey-Omura protocol
+encrypted_msg_receiver = mo_receiver.second_encryption_step(encrypted_msg_sender)
+
+# The double-encrypted message is sent back to the sender...
+# (transmission of encrypted_msg_receiver)
+
+# Sender's side again
+# -------------------
+# Perform the partial decryption step with Massey-Omura protocol
+partial_decrypted_msg = mo_sender.partial_decryption_step(encrypted_msg_receiver)
+
+# The partially decrypted message is sent back to the receiver...
+# (transmission of partial_decrypted_msg)
+
+# Receiver's final decryption
+# ---------------------------
+# Finish decryption with Massey-Omura protocol to get the original message
+original_message = mo_receiver.partial_decryption_step(partial_decrypted_msg)
+
+# Decode the message using the Koblitz method
+# `j` is used to resolve the mapping from the elliptic curve point back to the message
+decoded_message = koblitz.decode(original_message, j)
+
+# The decoded_message contains the original plaintext message
+print(decoded_message)
+```
+
+
 ## Documentation
 
-For more in-depth use and examples, check out the [official documentation](https://ecutils.readthedocs.io/en/latest/).
+For more in-depth use and examples, check out the [official documentation](https://ecutils.readthedocs.io/en/stable/).
 
 ## Support
 
 For issues, questions, or contributions, please refer to the project's [GitHub repository](https://github.com/isakruas/ecutils).
 
 ## License
```

### Comparing `ecutils-1.0.0/pyproject.toml` & `ecutils-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
   "Development Status :: 6 - Mature",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Build Tools",
   "Natural Language :: English",
 ]
@@ -29,21 +28,21 @@
   {name = "Isak Paulo de Andrade Ruas", email = "isakruas@gmail.com"},
   {name = "Celimar Reijane Alves Damasceno Paiva", email = "celimar.damasceno@ifnmg.edu.br"},
   {name = "Fernando Marcos Souza Silva", email = "fernando.silva@ifnmg.edu.br"},
 ]
 maintainers = [
   {name = "Isak Paulo de Andrade Ruas", email = "isakruas@gmail.com"}
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = []
 dynamic = ["version"]
 
 [project.urls]
-Homepage = "https://ecutils.readthedocs.io/en/latest/"
-Documentation = "https://ecutils.readthedocs.io/en/latest/"
+Homepage = "https://ecutils.readthedocs.io/en/stable/"
+Documentation = "https://ecutils.readthedocs.io/en/stable/"
 Repository = "https://github.com/isakruas/ecutils.git"
 "Bug Tracker" = "https://github.com/isakruas/ecutils/issues"
 Changelog = "https://github.com/isakruas/ecutils/blob/master/CHANGELOG.md"
 
 [tool.hatch.package]
 source-dir = "src"
```

