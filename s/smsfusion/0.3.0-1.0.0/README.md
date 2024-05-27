# Comparing `tmp/smsfusion-0.3.0-py3-none-any.whl.zip` & `tmp/smsfusion-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26740 bytes, number of entries: 17
+Zip file size: 26738 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 smsfusion/__about__.py
 -rw-r--r--  2.0 unx      241 b- defN 20-Feb-02 00:00 smsfusion/__init__.py
 -rw-r--r--  2.0 unx     9220 b- defN 20-Feb-02 00:00 smsfusion/_ahrs.py
 -rw-r--r--  2.0 unx    33165 b- defN 20-Feb-02 00:00 smsfusion/_ins.py
 -rw-r--r--  2.0 unx     9280 b- defN 20-Feb-02 00:00 smsfusion/_transforms.py
 -rw-r--r--  2.0 unx     2226 b- defN 20-Feb-02 00:00 smsfusion/_vectorops.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 smsfusion/benchmark/__init__.py
 -rw-r--r--  2.0 unx    24303 b- defN 20-Feb-02 00:00 smsfusion/benchmark/_benchmark.py
 -rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 smsfusion/calibrate/__init__.py
 -rw-r--r--  2.0 unx     2772 b- defN 20-Feb-02 00:00 smsfusion/calibrate/_calibrate.py
 -rw-r--r--  2.0 unx      235 b- defN 20-Feb-02 00:00 smsfusion/noise/__init__.py
 -rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 smsfusion/noise/_allan.py
 -rw-r--r--  2.0 unx    15163 b- defN 20-Feb-02 00:00 smsfusion/noise/_noise.py
-?rw-r--r--  2.0 unx      705 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1377 b- defN 20-Feb-02 00:00 smsfusion-0.3.0.dist-info/RECORD
-17 files, 102801 bytes uncompressed, 24488 bytes compressed:  76.2%
+?rw-r--r--  2.0 unx      705 b- defN 20-Feb-02 00:00 smsfusion-1.0.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 smsfusion-1.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1064 b- defN 20-Feb-02 00:00 smsfusion-1.0.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1377 b- defN 20-Feb-02 00:00 smsfusion-1.0.0.dist-info/RECORD
+17 files, 102801 bytes uncompressed, 24486 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: smsfusion/noise/_allan.py
 Comment: 
 
 Filename: smsfusion/noise/_noise.py
 Comment: 
 
-Filename: smsfusion-0.3.0.dist-info/METADATA
+Filename: smsfusion-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: smsfusion-0.3.0.dist-info/WHEEL
+Filename: smsfusion-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: smsfusion-0.3.0.dist-info/licenses/LICENSE
+Filename: smsfusion-1.0.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: smsfusion-0.3.0.dist-info/RECORD
+Filename: smsfusion-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smsfusion/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0"
+__version__ = "1.0.0"
```

## Comparing `smsfusion-0.3.0.dist-info/METADATA` & `smsfusion-1.0.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smsfusion
-Version: 0.3.0
+Version: 1.0.0
 Summary: Sensor fusion algorithms and utilities for SMS Motion
 Project-URL: Homepage, https://github.com/4Subsea/smsfusion-python
 Project-URL: Bug Tracker, https://github.com/4Subsea/smsfusion-python/issues
 Author-email: 4Subsea <python@4subsea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `smsfusion-0.3.0.dist-info/licenses/LICENSE` & `smsfusion-1.0.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `smsfusion-0.3.0.dist-info/RECORD` & `smsfusion-1.0.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-smsfusion/__about__.py,sha256=VrXpHDu3erkzwl_WXrqINBm9xWkcyUy53IQOj042dOs,22
+smsfusion/__about__.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
 smsfusion/__init__.py,sha256=KuSQtN5M1mBXyaN3g5pFCZ-qNEz0cM88AJIC_MU9-I4,241
 smsfusion/_ahrs.py,sha256=ByD2KGv0HKODfBpBWeeAj6W0dTmkfQkIk4CZm1zD9g0,9220
 smsfusion/_ins.py,sha256=mccnRPXGTnIF3qGrGih37SbW7mD8AlVSLCst3bdH-kw,33165
 smsfusion/_transforms.py,sha256=S3vH3b7_tuohQLMStK6cLrffGm5mXTFj1TFvsoRtMJo,9280
 smsfusion/_vectorops.py,sha256=F6xDYgVMxU9Fo7xFQvKy7UnaBohpDBuFBHzUIjnmz-k,2226
 smsfusion/benchmark/__init__.py,sha256=m1daVGbSVG1MwgwQM28YJi1Sj1c0CdfPsxIEhPEOWoA,489
 smsfusion/benchmark/_benchmark.py,sha256=5j8Rr-mK5jxJDvNE3oBv5q-dhojVBGqQ8gUDt9H-tqc,24303
 smsfusion/calibrate/__init__.py,sha256=qZ37Ct8DLaxnF-xoagAixCzXD8VSNHe40Uv5jG7wJkk,83
 smsfusion/calibrate/_calibrate.py,sha256=pmD9TJQ8UYuBSm5sXfsF6FfHpjMV45gUYhd9XwwUnxM,2772
 smsfusion/noise/__init__.py,sha256=C5AIH5THPxkb2xmyoTo2eVBCuSFChdNdUGF639nBUus,235
 smsfusion/noise/_allan.py,sha256=JonvSQTviEPQfDEpZg9OWYEOl3sYzG5uB-afqrMV39s,2369
 smsfusion/noise/_noise.py,sha256=njKiHKAmD25FCyX0uBY1oQdTIeIWNPrk3SwPtY5qfFY,15163
-smsfusion-0.3.0.dist-info/METADATA,sha256=sR_hx6Km0TvPOV0aiCV56lMo99FSli33urGWwLZYjaQ,705
-smsfusion-0.3.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-smsfusion-0.3.0.dist-info/licenses/LICENSE,sha256=oEQkXxrh0POZZPEv5oYwkmLuh-USLG0uH2JiaThmjA0,1064
-smsfusion-0.3.0.dist-info/RECORD,,
+smsfusion-1.0.0.dist-info/METADATA,sha256=nsKZ5wPTWldyqykP6FdpyipffNyqjwx5pyxAvx3DQlE,705
+smsfusion-1.0.0.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+smsfusion-1.0.0.dist-info/licenses/LICENSE,sha256=oEQkXxrh0POZZPEv5oYwkmLuh-USLG0uH2JiaThmjA0,1064
+smsfusion-1.0.0.dist-info/RECORD,,
```

