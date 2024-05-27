# Comparing `tmp/brickbundles-0.8.2-py3-none-any.whl.zip` & `tmp/brickbundles-0.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -279,11 +279,11 @@
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.8.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32052 b- defN 16-Jan-01 00:00 brickbundles-0.8.2.dist-info/RECORD
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.8.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.8.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32052 b- defN 16-Jan-01 00:00 brickbundles-0.8.3.dist-info/RECORD
 287 files, 139784 bytes uncompressed, 61305 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -846,17 +846,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.8.2.dist-info/METADATA
+Filename: brickbundles-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.8.2.dist-info/WHEEL
+Filename: brickbundles-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.8.2.dist-info/RECORD
+Filename: brickbundles-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `brickbundles-0.8.2.dist-info/METADATA` & `brickbundles-0.8.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.8.2
+Version: 0.8.3
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.8.2.dist-info/RECORD` & `brickbundles-0.8.3.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -278,10 +278,10 @@
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.8.2.dist-info/METADATA,sha256=qDIafX6XpHay92zG8pT9ijUF1jDphC3jO2QmnWSB0U0,1066
-brickbundles-0.8.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.8.2.dist-info/RECORD,,
+brickbundles-0.8.3.dist-info/METADATA,sha256=sQfVVLp4GOuRGH2sthf6um3iBylh8AhRljizPM7kRVg,1066
+brickbundles-0.8.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.8.3.dist-info/RECORD,,
```

