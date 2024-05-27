# Comparing `tmp/bootpay-backend-2.0.8.tar.gz` & `tmp/bootpay_backend-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootpay-backend-2.0.8.tar", last modified: Wed Mar 22 06:22:49 2023, max compression
+gzip compressed data, was "bootpay_backend-2.0.9.tar", last modified: Mon May 27 07:43:49 2024, max compression
```

## Comparing `bootpay-backend-2.0.8.tar` & `bootpay_backend-2.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ehowlsla   (501) staff       (20)        0 2023-03-22 06:22:49.514945 bootpay-backend-2.0.8/
--rw-r--r--   0 ehowlsla   (501) staff       (20)     1063 2022-05-23 01:08:57.000000 bootpay-backend-2.0.8/LICENSE
--rw-r--r--   0 ehowlsla   (501) staff       (20)    14154 2023-03-22 06:22:49.515095 bootpay-backend-2.0.8/PKG-INFO
--rw-r--r--   0 ehowlsla   (501) staff       (20)    12917 2022-09-13 07:47:17.000000 bootpay-backend-2.0.8/README.md
-drwxr-xr-x   0 ehowlsla   (501) staff       (20)        0 2023-03-22 06:22:49.512522 bootpay-backend-2.0.8/bootpay_backend/
--rw-r--r--   0 ehowlsla   (501) staff       (20)       70 2022-05-23 01:08:57.000000 bootpay-backend-2.0.8/bootpay_backend/__init__.py
--rw-r--r--   0 ehowlsla   (501) staff       (20)      447 2022-05-23 01:08:57.000000 bootpay-backend-2.0.8/bootpay_backend/bankcode.py
--rw-r--r--   0 ehowlsla   (501) staff       (20)    12125 2023-03-22 06:13:26.000000 bootpay-backend-2.0.8/bootpay_backend/rest_client.py
-drwxr-xr-x   0 ehowlsla   (501) staff       (20)        0 2023-03-22 06:22:49.514639 bootpay-backend-2.0.8/bootpay_backend.egg-info/
--rw-r--r--   0 ehowlsla   (501) staff       (20)    14154 2023-03-22 06:22:49.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/PKG-INFO
--rw-r--r--   0 ehowlsla   (501) staff       (20)      355 2023-03-22 06:22:49.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/SOURCES.txt
--rw-r--r--   0 ehowlsla   (501) staff       (20)        1 2023-03-22 06:22:49.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/dependency_links.txt
--rw-r--r--   0 ehowlsla   (501) staff       (20)        1 2022-06-28 05:49:57.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/not-zip-safe
--rw-r--r--   0 ehowlsla   (501) staff       (20)       95 2023-03-22 06:22:49.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/requires.txt
--rw-r--r--   0 ehowlsla   (501) staff       (20)       16 2023-03-22 06:22:49.000000 bootpay-backend-2.0.8/bootpay_backend.egg-info/top_level.txt
--rw-r--r--   0 ehowlsla   (501) staff       (20)       79 2023-03-22 06:22:49.515775 bootpay-backend-2.0.8/setup.cfg
--rw-r--r--   0 ehowlsla   (501) staff       (20)     1833 2023-03-22 06:19:38.000000 bootpay-backend-2.0.8/setup.py
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.927452 bootpay_backend-2.0.9/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)     1063 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/LICENSE
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-27 07:43:49.927297 bootpay_backend-2.0.9/PKG-INFO
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    12917 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/README.md
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.925871 bootpay_backend-2.0.9/bootpay_backend/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       70 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/bootpay_backend/__init__.py
+-rw-r--r--   0 taesupyoon   (501) staff       (20)      447 2024-05-27 06:11:15.000000 bootpay_backend-2.0.9/bootpay_backend/bankcode.py
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    14014 2024-05-27 07:12:15.000000 bootpay_backend-2.0.9/bootpay_backend/rest_client.py
+drwxr-xr-x   0 taesupyoon   (501) staff       (20)        0 2024-05-27 07:43:49.927068 bootpay_backend-2.0.9/bootpay_backend.egg-info/
+-rw-r--r--   0 taesupyoon   (501) staff       (20)    14273 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/PKG-INFO
+-rw-r--r--   0 taesupyoon   (501) staff       (20)      355 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)        1 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/not-zip-safe
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       95 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/requires.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       16 2024-05-27 07:43:49.000000 bootpay_backend-2.0.9/bootpay_backend.egg-info/top_level.txt
+-rw-r--r--   0 taesupyoon   (501) staff       (20)       79 2024-05-27 07:43:49.927633 bootpay_backend-2.0.9/setup.cfg
+-rw-r--r--   0 taesupyoon   (501) staff       (20)     1833 2024-05-27 07:40:44.000000 bootpay_backend-2.0.9/setup.py
```

### Comparing `bootpay-backend-2.0.8/LICENSE` & `bootpay_backend-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bootpay-backend-2.0.8/PKG-INFO` & `bootpay_backend-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootpay-backend
-Version: 2.0.8
+Version: 2.0.9
 Summary: bootpay server side plugin for python
 Home-page: https://github.com/bootpay/backend-python/tree/2-x-development
 Author: bootpay <bootpay.co.kr@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.20; python_version >= "3.0"
+Requires-Dist: requests[security]>=2.20; python_version < "3.0"
 
 
 ## Bootpay Python Server Side Library
 부트페이 공식 파이썬 라이브러리 입니다 (서버사이드 용)
 
 Python 언어로 작성된 어플리케이션, 프레임워크 등에서 사용가능합니다.
```

### Comparing `bootpay-backend-2.0.8/README.md` & `bootpay_backend-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bootpay-backend-2.0.8/bootpay_backend/rest_client.py` & `bootpay_backend-2.0.9/bootpay_backend/rest_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 class BootpayBackend:
     BASE_URL = {
         'development': 'https://dev-api.bootpay.co.kr/v2',
         'stage': 'https://stage-api.bootpay.co.kr/v2',
         'production': 'https://api.bootpay.co.kr/v2'
     }
-    API_VERSION = '4.2.9'
-    SDK_VERSION = '2.0.7'
+    API_VERSION = '5.0.0'
+    SDK_VERSION = '2.0.9'
 
     def __init__(self, application_id, private_key, mode='production'):
         self.application_id = application_id
         self.private_key = private_key
         self.mode = mode
         self.token = None
         self.api_version = self.API_VERSION
@@ -58,16 +58,17 @@
         if 'error_code' not in response:
             self.token = response['access_token']
         return response
 
     # Get Receipt Payment Data
     # Comment by GOSOMI
     # @param receipt_id: string
-    def receipt_payment(self, receipt_id=''):
-        return self.__request(method='get', url=self.__entrypoints(f'receipt/{receipt_id}'))
+    def receipt_payment(self, receipt_id='', lookup_user_data=False):
+        return self.__request(method='get', url=self.__entrypoints(
+            f'receipt/{receipt_id}?lookup_user_data={lookup_user_data and "true" or "false"}'))
 
     # certificate
     # Comment by GOSOMI
     # @param receipt_id: string
     def certificate(self, receipt_id=''):
         return self.__request(method='get', url=self.__entrypoints(f'certificate/{receipt_id}'))
 
@@ -79,14 +80,22 @@
 
     # lookup subscribe billing key
     # Comment by GOSOMI
     # @param receipt_id:string
     def lookup_subscribe_billing_key(self, receipt_id=''):
         return self.__request(method='get', url=self.__entrypoints(f'subscribe/billing_key/{receipt_id}'))
 
+
+    # lookup billing key by billing_key
+    # Comment by ehowlsla
+    # @param billing_key:string
+    def lookup_billing_key(self,  billing_key=''):
+        return self.__request(method='get', url=self.__entrypoints(f'billing_key/{billing_key}'))
+
+
     # request subscribe billing key
     # Comment by GOSOMI
     def request_subscribe_billing_key(self, pg='', order_name='', subscription_id='', card_no='', card_pw='',
                                       card_identity_no='', card_expire_year='', card_expire_month='', price=0,
                                       tax_free=0, extra=None, user=None, metadata=None):
         return self.__request(method='post', url=self.__entrypoints('request/subscribe'), data={
             "pg": pg,
@@ -301,7 +310,38 @@
         return self.__request(
             method='post',
             url=self.__entrypoints('authenticate/realarm'),
             data={
                 "receipt_id": receipt_id
             }
         )
+
+    # 계좌 자동 결제를 위한 빌링키 발급
+    def request_subscribe_automatic_transfer_billing_key(self, pg='', order_name='', price=None, tax_free=None, subscription_id='',
+                                                         extra=None, user=None, metadata=None, auth_type='ARS', username='',
+                                                         bank_name='', bank_account='', identity_no='', cash_receipt_type='소득공제',
+                                                         cash_receipt_identity_no=None, phone=''):
+        return self.__request(method='post', url=self.__entrypoints('request/subscribe/automatic-transfer'), data={
+            "pg": pg,
+            "order_name": order_name,
+            "subscription_id": subscription_id,
+            "price": price,
+            "tax_free": tax_free,
+            "extra": extra,
+            "user": user,
+            "metadata": metadata,
+            "auth_type": auth_type,
+            "username": username,
+            "bank_name": bank_name,
+            "bank_account": bank_account,
+            "identity_no": identity_no,
+            "cash_receipt_type": cash_receipt_type,
+            "cash_receipt_identity_no": cash_receipt_identity_no,
+            "phone": phone,
+        })
+
+
+    # 출금 동의 확인 요청
+    def publish_automatic_transfer_billing_key(self, receipt_id=''):
+        return self.__request(method='post', url=self.__entrypoints('request/subscribe/automatic-transfer/publish'), data={
+            "receipt_id": receipt_id
+        })
```

### Comparing `bootpay-backend-2.0.8/bootpay_backend.egg-info/PKG-INFO` & `bootpay_backend-2.0.9/bootpay_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootpay-backend
-Version: 2.0.8
+Version: 2.0.9
 Summary: bootpay server side plugin for python
 Home-page: https://github.com/bootpay/backend-python/tree/2-x-development
 Author: bootpay <bootpay.co.kr@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.20; python_version >= "3.0"
+Requires-Dist: requests[security]>=2.20; python_version < "3.0"
 
 
 ## Bootpay Python Server Side Library
 부트페이 공식 파이썬 라이브러리 입니다 (서버사이드 용)
 
 Python 언어로 작성된 어플리케이션, 프레임워크 등에서 사용가능합니다.
```

### Comparing `bootpay-backend-2.0.8/setup.py` & `bootpay_backend-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name = 'bootpay-backend',
-    version = '2.0.8',
+    version = '2.0.9',
     description = 'bootpay server side plugin for python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'bootpay <bootpay.co.kr@gmail.com>',
     packages = setuptools.find_packages(),
     keyword = ['pg', '결제연동', 'bootpay', 'payment'],
     install_requires=[
```

