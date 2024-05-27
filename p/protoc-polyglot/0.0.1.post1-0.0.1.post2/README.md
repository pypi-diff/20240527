# Comparing `tmp/protoc_polyglot-0.0.1.post1-py3-none-any.whl.zip` & `tmp/protoc_polyglot-0.0.1.post2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -7,11 +7,11 @@
 -rwxr-xr-x  2.0 unx      656 b- defN 20-Feb-02 00:00 core/java/cli.py
 -rwxr-xr-x  2.0 unx      627 b- defN 20-Feb-02 00:00 core/js/cli.py
 -rwxr-xr-x  2.0 unx      576 b- defN 20-Feb-02 00:00 core/obj-c/cli.py
 -rwxr-xr-x  2.0 unx      540 b- defN 20-Feb-02 00:00 core/php/cli.py
 -rwxr-xr-x  2.0 unx      626 b- defN 20-Feb-02 00:00 core/python/cli.py
 -rwxr-xr-x  2.0 unx      557 b- defN 20-Feb-02 00:00 core/ruby/cli.py
 -rwxr-xr-x  2.0 unx      615 b- defN 20-Feb-02 00:00 core/rust/cli.py
-?rw-r--r--  2.0 unx     3023 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1107 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post1.dist-info/RECORD
+?rw-r--r--  2.0 unx     3023 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1107 b- defN 20-Feb-02 00:00 protoc_polyglot-0.0.1.post2.dist-info/RECORD
 15 files, 18120 bytes uncompressed, 8050 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -30,17 +30,17 @@
 
 Filename: core/ruby/cli.py
 Comment: 
 
 Filename: core/rust/cli.py
 Comment: 
 
-Filename: protoc_polyglot-0.0.1.post1.dist-info/METADATA
+Filename: protoc_polyglot-0.0.1.post2.dist-info/METADATA
 Comment: 
 
-Filename: protoc_polyglot-0.0.1.post1.dist-info/WHEEL
+Filename: protoc_polyglot-0.0.1.post2.dist-info/WHEEL
 Comment: 
 
-Filename: protoc_polyglot-0.0.1.post1.dist-info/RECORD
+Filename: protoc_polyglot-0.0.1.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `protoc_polyglot-0.0.1.post1.dist-info/METADATA` & `protoc_polyglot-0.0.1.post2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: protoc_polyglot
-Version: 0.0.1.post1
+Version: 0.0.1.post2
 Summary: Protoc wrapper for compilation into any language
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Milan Pultar <milan.pultar@gmail.com>, Hugo Kunák <author@example.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `protoc_polyglot-0.0.1.post1.dist-info/RECORD` & `protoc_polyglot-0.0.1.post2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -6,10 +6,10 @@
 core/java/cli.py,sha256=lpBamH4gbulBHrxhvV_qtE7tq9Umb8s1FoRXzYd6LRc,656
 core/js/cli.py,sha256=W8BHSj8qkMyfId4Yvg0WY7sDaAtbZ6PHAjyPXsu5o8Y,627
 core/obj-c/cli.py,sha256=JoTF3ha37tBpVXmg5QHpcRXN1JKCFY7mCPl7Vg7QzJo,576
 core/php/cli.py,sha256=ma-cJpb-ehSsrrWWhBjYMSAGxGyP6sy7WcCbEmUC12U,540
 core/python/cli.py,sha256=ukh0Eh4yotTB1MCyHf3Hc6FW79BskVuSzZb96TN2fe0,626
 core/ruby/cli.py,sha256=MWUxzja5wedKochARssPOSEzOau9rGY65EC3jWdiOsI,557
 core/rust/cli.py,sha256=Y2OV_vL8j5faZabswMzvUEHjbxS6tU2S-L0nqpVxWvk,615
-protoc_polyglot-0.0.1.post1.dist-info/METADATA,sha256=gkt4MMpvC1Vh1ts7MaPR8pkM0PdGK2XukVgUkafaimg,3023
-protoc_polyglot-0.0.1.post1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-protoc_polyglot-0.0.1.post1.dist-info/RECORD,,
+protoc_polyglot-0.0.1.post2.dist-info/METADATA,sha256=VeDse0-FfzvzmjOPSM31lqlT-Ohbl4K6GGA5LM7e31w,3023
+protoc_polyglot-0.0.1.post2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+protoc_polyglot-0.0.1.post2.dist-info/RECORD,,
```

