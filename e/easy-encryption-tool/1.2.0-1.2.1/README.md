# Comparing `tmp/easy_encryption_tool-1.2.0-py3-none-any.whl.zip` & `tmp/easy_encryption_tool-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 45039 bytes, number of entries: 16
+Zip file size: 45477 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      253 b- defN 24-Apr-04 15:14 easy_encryption_tool/__init__.py
 -rw-r--r--  2.0 unx    20027 b- defN 24-Apr-04 15:39 easy_encryption_tool/aes_command.py
 -rw-r--r--  2.0 unx    13951 b- defN 24-Apr-06 06:57 easy_encryption_tool/cert_parse.py
 -rw-r--r--  2.0 unx      702 b- defN 24-Apr-04 08:28 easy_encryption_tool/command_perf.py
 -rw-r--r--  2.0 unx     7420 b- defN 24-Apr-05 05:45 easy_encryption_tool/common.py
 -rw-r--r--  2.0 unx    12652 b- defN 24-Apr-04 15:39 easy_encryption_tool/ecc_command.py
 -rw-r--r--  2.0 unx     4111 b- defN 24-Apr-04 15:39 easy_encryption_tool/hmac_command.py
 -rw-r--r--  2.0 unx     2284 b- defN 24-Apr-05 16:06 easy_encryption_tool/main.py
 -rw-r--r--  2.0 unx     2675 b- defN 24-Apr-05 05:45 easy_encryption_tool/random_str.py
--rw-r--r--  2.0 unx    17736 b- defN 24-Apr-04 15:39 easy_encryption_tool/rsa_command.py
+-rw-r--r--  2.0 unx    19223 b- defN 24-May-27 15:57 easy_encryption_tool/rsa_command.py
 -rw-r--r--  2.0 unx      870 b- defN 24-Apr-05 05:45 easy_encryption_tool/tool_version.py
--rw-r--r--  2.0 unx    67547 b- defN 24-Apr-06 07:07 easy_encryption_tool-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 07:07 easy_encryption_tool-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 24-Apr-06 07:07 easy_encryption_tool-1.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       21 b- defN 24-Apr-06 07:07 easy_encryption_tool-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1458 b- defN 24-Apr-06 07:07 easy_encryption_tool-1.2.0.dist-info/RECORD
-16 files, 151882 bytes uncompressed, 42593 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx    67547 b- defN 24-May-27 16:06 easy_encryption_tool-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 16:06 easy_encryption_tool-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 24-May-27 16:06 easy_encryption_tool-1.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 24-May-27 16:06 easy_encryption_tool-1.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1458 b- defN 24-May-27 16:06 easy_encryption_tool-1.2.1.dist-info/RECORD
+16 files, 153369 bytes uncompressed, 43031 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: easy_encryption_tool/rsa_command.py
 Comment: 
 
 Filename: easy_encryption_tool/tool_version.py
 Comment: 
 
-Filename: easy_encryption_tool-1.2.0.dist-info/METADATA
+Filename: easy_encryption_tool-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: easy_encryption_tool-1.2.0.dist-info/WHEEL
+Filename: easy_encryption_tool-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: easy_encryption_tool-1.2.0.dist-info/entry_points.txt
+Filename: easy_encryption_tool-1.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.2.0.dist-info/top_level.txt
+Filename: easy_encryption_tool-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: easy_encryption_tool-1.2.0.dist-info/RECORD
+Filename: easy_encryption_tool-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## easy_encryption_tool/rsa_command.py

```diff
@@ -4,16 +4,15 @@
 import base64
 
 import click
 from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 
-from easy_encryption_tool import command_perf
-from easy_encryption_tool import common
+from easy_encryption_tool import command_perf, common
 
 rsa_key_size = ['2048', '3072', '4096']
 rsa_encryption_mode = ['oaep', 'pkcs1v15']
 rsa_sign_mode = ['pss', 'pkcs1v15']
 
 rsa_hash_map = {
     hashes.SHA256().name: hashes.SHA256,
@@ -23,14 +22,20 @@
     # cryptography库的当前不支持使用SHA3-512哈希算法与OAEP填充模式的组合
     # hashes.SHA3_224().name: hashes.SHA3_224,
     # hashes.SHA3_256().name: hashes.SHA3_256,
     # hashes.SHA3_384().name: hashes.SHA3_384,
     # ashes.SHA3_512().name: hashes.SHA3_512,
 }
 
+rsa_digest_size_map = {
+    hashes.SHA256().name: hashes.SHA256().digest_size,
+    hashes.SHA384().name: hashes.SHA384().digest_size,
+    hashes.SHA512().name: hashes.SHA512().digest_size,
+}
+
 
 @click.group(name = 'rsa', short_help = 'rsa加解密和签名验签工具')
 def rsa_group():
     pass
 
 
 @click.command(name = 'generate')
@@ -91,14 +96,29 @@
 
 def combine_if_not_empty(hash_mode: str, mode: str) -> str:
     if len(hash_mode) <= 0:
         return mode
     return '{}-{}'.format(mode, hash_mode)
 
 
+def get_encryption_max_plain_length(mode: str, key_length: int, hash_length: int) -> int:
+    """
+    对于 OAEP（Optimal Asymmetric Encryption Padding）填充方案，
+    如果使用的是 SHA-256 哈希函数，那么明文的最大长度等于密钥长度减去 2 倍的哈希长度再减去 2。
+    例如，如果你使用的是 2048 位的 RSA 密钥，那么明文的最大长度就是 256 字节（2048 位）减去 2*32 字节（SHA-256 的输出长度）再减去 2，即 190 字节。
+    对于 PKCS#1 v1.5 填充方案，明文的最大长度等于密钥长度减去 11 字节（这是为了留出足够的空间来存放必要的填充数据）。
+    例如，如果你使用的是 2048 位的 RSA 密钥，那么明文的最大长度就是 256 字节（2048 位）减去 11 字节，即 245 字节。
+    """
+    if mode == 'oaep':
+        return key_length - 2 * hash_length - 2
+    if mode == 'pkcs1v15':
+        return key_length - 11
+    pass
+
+
 @click.command(name = 'encrypt')
 @click.option('-f', '--public-key',
               required = True,
               type = click.STRING,
               help = '公钥文件路径')
 @click.option('-i', '--input-data',
               required = True,
@@ -154,28 +174,35 @@
             'the data exceeds the maximum bytes limit, limited to:{}Bytes, now:{}Bytes'.format(input_limit * 1024 * 1024,
                                                                                                len(input_raw_bytes)))
         return
 
     pub_key = common.load_public_key(encoding = encoding, file_path = public_key)
     if pub_key is None:
         return
+    max_plain_size = get_encryption_max_plain_length(mode, pub_key.key_size // 8,
+                                                     rsa_digest_size_map[hash_mode])
+    click.echo(
+        'rsa key size:{} bytes, hash digest size:{} bytes, allowed max plain size:{} bytes, input plain:{} bytes'.format(
+            pub_key.key_size, rsa_digest_size_map[hash_mode], max_plain_size, len(input_raw_bytes)
+        ))
+    if len(input_raw_bytes) > max_plain_size:
+        return
     cipher = None
     if mode == 'oaep':
         rsa_oaep_padding = padding.OAEP(
             mgf = padding.MGF1(algorithm = rsa_hash_map[hash_mode]()),
             algorithm = rsa_hash_map[hash_mode](),
             label = None,
         )
         cipher = pub_key.encrypt(plaintext = input_raw_bytes, padding = rsa_oaep_padding)
     if mode == 'pkcs1v15':
         hash_mode = ''
         cipher = pub_key.encrypt(plaintext = input_raw_bytes, padding = padding.PKCS1v15())
-    click.echo('pub key size:{}\npadding mode:{}\ncipher:{}'.format(pub_key.key_size,
-                                                                    combine_if_not_empty(hash_mode, mode),
-                                                                    base64.b64encode(cipher).decode('utf-8')))
+    click.echo('padding mode:{}\ncipher:{}'.format(combine_if_not_empty(hash_mode, mode),
+                                                   base64.b64encode(cipher).decode('utf-8')))
     return
 
 
 @click.command(name = 'decrypt')
 @click.option('-f', '--private-key',
               required = True,
               type = click.STRING,
```

## Comparing `easy_encryption_tool-1.2.0.dist-info/METADATA` & `easy_encryption_tool-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-encryption-tool
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://cloud.tencent.com/developer/article/2404712
 Author: bowenerchen
 Author-email: bowener.chen@gmail.com
 License: MIT
 Keywords: encryption cli tool security aes hmac ecc rsa
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `easy_encryption_tool-1.2.0.dist-info/RECORD` & `easy_encryption_tool-1.2.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 easy_encryption_tool/cert_parse.py,sha256=z06Vw9-e6MviEVytt8RsEH67zuXjN5HgWvnCm56Kllc,13951
 easy_encryption_tool/command_perf.py,sha256=cMRgLVDiu9qdjVDXEl-WOOi1iNfWVu56Ee_tLC_6hOE,702
 easy_encryption_tool/common.py,sha256=vY5pMJsCOwK8sej5NXWr2ScSg7w2FJLlYkncawji8sM,7420
 easy_encryption_tool/ecc_command.py,sha256=g76LOqS-UILqXSgFZhqw_1qAXpXDZRUNslcmAQHmkpk,12652
 easy_encryption_tool/hmac_command.py,sha256=mQaZ9dDsh3q4KNEhkyht8bVPcT5LD0Oq8b2tEpqxWKg,4111
 easy_encryption_tool/main.py,sha256=c5iXQa3r2Sq1U6O8UX_9XyE_PrFb1NHz-EYzCk2Ye34,2284
 easy_encryption_tool/random_str.py,sha256=Mz8QkU8w-TrKWxLKhevXtic9_EPryeYlJcrEhXaQcVA,2675
-easy_encryption_tool/rsa_command.py,sha256=QsAJUo69Yo8EpZ3mbu4mbIR50NGPoRXfzZPtHJAOIGg,17736
+easy_encryption_tool/rsa_command.py,sha256=F9tMquWs6vKq7vqW5FhGjEbn6fK33_ci_Nvo7fpYe98,19223
 easy_encryption_tool/tool_version.py,sha256=Gz2mCkhX1Ztrpr_TaTBkyVWs9Yk3gX8QxxlgkB4ga0A,870
-easy_encryption_tool-1.2.0.dist-info/METADATA,sha256=ZbIjDDdKPos85QOrYA_N4gPE1NXyZpyxJ4xrzCYi538,67547
-easy_encryption_tool-1.2.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-easy_encryption_tool-1.2.0.dist-info/entry_points.txt,sha256=qrNi4Ml3z53yoZNoOEQFVofyZCmLG_sUQSytiejkJYY,83
-easy_encryption_tool-1.2.0.dist-info/top_level.txt,sha256=2RdeCo7jNerQyfXisv2UZytrMsfSAwsyef13Mq3TkMU,21
-easy_encryption_tool-1.2.0.dist-info/RECORD,,
+easy_encryption_tool-1.2.1.dist-info/METADATA,sha256=qRNNUTpDgogMuBKKuj722adfxHpxhHfDBY5Zg_VoL18,67547
+easy_encryption_tool-1.2.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+easy_encryption_tool-1.2.1.dist-info/entry_points.txt,sha256=qrNi4Ml3z53yoZNoOEQFVofyZCmLG_sUQSytiejkJYY,83
+easy_encryption_tool-1.2.1.dist-info/top_level.txt,sha256=2RdeCo7jNerQyfXisv2UZytrMsfSAwsyef13Mq3TkMU,21
+easy_encryption_tool-1.2.1.dist-info/RECORD,,
```

