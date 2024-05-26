# Comparing `tmp/maesyorikun-0.1.1-py3-none-any.whl.zip` & `tmp/maesyorikun-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3744 bytes, number of entries: 7
--rw-r--r--  2.0 unx      222 b- defN 24-May-26 22:15 maesyorikun/__init__.py
+Zip file size: 4460 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      222 b- defN 24-May-26 22:25 maesyorikun/__init__.py
 -rw-r--r--  2.0 unx     7443 b- defN 24-May-26 21:00 maesyorikun/maesyorikun.py
 -rw-r--r--  2.0 unx      135 b- defN 24-May-26 21:17 maesyorikun/test.py
--rw-r--r--  2.0 unx      493 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 24-May-26 22:16 maesyorikun-0.1.1.dist-info/RECORD
-7 files, 8947 bytes uncompressed, 2766 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     1747 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      551 b- defN 24-May-26 22:25 maesyorikun-0.1.2.dist-info/RECORD
+7 files, 10202 bytes uncompressed, 3482 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: maesyorikun/maesyorikun.py
 Comment: 
 
 Filename: maesyorikun/test.py
 Comment: 
 
-Filename: maesyorikun-0.1.1.dist-info/METADATA
+Filename: maesyorikun-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: maesyorikun-0.1.1.dist-info/WHEEL
+Filename: maesyorikun-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: maesyorikun-0.1.1.dist-info/top_level.txt
+Filename: maesyorikun-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: maesyorikun-0.1.1.dist-info/RECORD
+Filename: maesyorikun-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## maesyorikun/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .maesyorikun import *
 
 __copyright__    = 'Copyright (C) 2024 makimoto eita'
-__version__      = '0.1.1'
+__version__      = '0.1.2'
 __author__       = 'Makimoto-eita'
 __author_email__ = 's2222034@stu.musahino-u.ac.jp'
 
 __all__ = ['maesyorikun']
```

## Comparing `maesyorikun-0.1.1.dist-info/RECORD` & `maesyorikun-0.1.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-maesyorikun/__init__.py,sha256=ORoAU0jndIcTX06kxCsW1cL4kFxetQU9c1ISwBbDZUo,222
+maesyorikun/__init__.py,sha256=Gi4cLlCX20JVPP6T7h5e1JFgFpqAMVIMVnhk_zHPcKE,222
 maesyorikun/maesyorikun.py,sha256=gk73QcxcopgLHPAcMKPjUV08XegoUab8UfvY9RGZ1P4,7443
 maesyorikun/test.py,sha256=eaErmSUErtup4maJqwR8ld9DLC_Qb6SAyiC-JNIqMgQ,135
-maesyorikun-0.1.1.dist-info/METADATA,sha256=N5nt-hu9gIf5laZydcvl_u5l43_yxVgD2fN08V5Req4,493
-maesyorikun-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-maesyorikun-0.1.1.dist-info/top_level.txt,sha256=DzsklxK_SdkSBsrCphKSEvjJUHqGaPBPTwkgbl88eOw,12
-maesyorikun-0.1.1.dist-info/RECORD,,
+maesyorikun-0.1.2.dist-info/METADATA,sha256=V2W2-i2tK83Ylg-a_FgVzcNMYfTUjMXVdgeGsFdu-Jo,1747
+maesyorikun-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+maesyorikun-0.1.2.dist-info/top_level.txt,sha256=DzsklxK_SdkSBsrCphKSEvjJUHqGaPBPTwkgbl88eOw,12
+maesyorikun-0.1.2.dist-info/RECORD,,
```

