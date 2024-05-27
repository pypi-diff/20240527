# Comparing `tmp/rocketmq-client-python-mi-1.0.1.tar.gz` & `tmp/rocketmq-client-python-mi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mi/project/sdk/rocketmq-client-python/dist/tmpy5mppufv/rocketmq-client-python-mi-1.0.1.tar", last modified: Fri Mar 11 03:14:20 2022, max compression
+gzip compressed data, was "rocketmq-client-python-mi-1.0.2.tar", last modified: Mon May 27 12:27:34 2024, max compression
```

## Comparing `rocketmq-client-python-mi-1.0.1.tar` & `rocketmq-client-python-mi-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/
--rw-rw-r--   0 mi        (1000) mi        (1000)    11333 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/LICENSE
--rw-rw-r--   0 mi        (1000) mi        (1000)     2787 2022-01-27 06:07:16.000000 rocketmq-client-python-mi-1.0.1/README.md
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/
--rw-rw-r--   0 mi        (1000) mi        (1000)        1 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)     3547 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)       35 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/requires.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       17 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/top_level.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)      457 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)     3547 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)      169 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/NOTICE
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/rocketmq/
--rw-rw-r--   0 mi        (1000) mi        (1000)      810 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/rocketmq/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    16402 2022-01-27 03:04:25.000000 rocketmq-client-python-mi-1.0.1/rocketmq/client.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    11189 2022-03-11 03:06:25.000000 rocketmq-client-python-mi-1.0.1/rocketmq/ffi.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1599 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/rocketmq/consts.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2588 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/rocketmq/exceptions.py
--rwxrwxr-x   0 mi        (1000) mi        (1000)     2948 2022-03-11 03:11:02.000000 rocketmq-client-python-mi-1.0.1/setup.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      256 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/setup.cfg
--rw-rw-r--   0 mi        (1000) mi        (1000)      175 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/MANIFEST.in
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-03-11 03:14:20.000000 rocketmq-client-python-mi-1.0.1/samples/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1458 2022-01-27 06:59:29.000000 rocketmq-client-python-mi-1.0.1/samples/consumer.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3648 2022-01-27 02:23:27.000000 rocketmq-client-python-mi-1.0.1/samples/producer.py
--rw-rw-r--   0 mi        (1000) mi        (1000)        0 2021-12-24 08:33:55.000000 rocketmq-client-python-mi-1.0.1/samples/__init__.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2024-05-27 12:27:34.271828 rocketmq-client-python-mi-1.0.2/
+-rw-r--r--   0 humkum     (501) staff       (20)    11333 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/LICENSE
+-rw-r--r--   0 humkum     (501) staff       (20)      175 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/MANIFEST.in
+-rw-r--r--   0 humkum     (501) staff       (20)      169 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/NOTICE
+-rw-r--r--   0 humkum     (501) staff       (20)     3803 2024-05-27 12:27:34.271892 rocketmq-client-python-mi-1.0.2/PKG-INFO
+-rw-r--r--   0 humkum     (501) staff       (20)     3043 2024-05-27 12:25:01.000000 rocketmq-client-python-mi-1.0.2/README.md
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2024-05-27 12:27:34.269996 rocketmq-client-python-mi-1.0.2/rocketmq/
+-rw-r--r--   0 humkum     (501) staff       (20)      810 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/rocketmq/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)    16706 2024-05-27 12:25:01.000000 rocketmq-client-python-mi-1.0.2/rocketmq/client.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1599 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/rocketmq/consts.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3792 2024-05-27 12:25:01.000000 rocketmq-client-python-mi-1.0.2/rocketmq/exceptions.py
+-rw-r--r--   0 humkum     (501) staff       (20)    12498 2024-05-27 12:25:01.000000 rocketmq-client-python-mi-1.0.2/rocketmq/ffi.py
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2024-05-27 12:27:34.270963 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/
+-rw-r--r--   0 humkum     (501) staff       (20)     3803 2024-05-27 12:27:34.000000 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/PKG-INFO
+-rw-r--r--   0 humkum     (501) staff       (20)      457 2024-05-27 12:27:34.000000 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/SOURCES.txt
+-rw-r--r--   0 humkum     (501) staff       (20)        1 2024-05-27 12:27:34.000000 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/dependency_links.txt
+-rw-r--r--   0 humkum     (501) staff       (20)       35 2024-05-27 12:27:34.000000 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/requires.txt
+-rw-r--r--   0 humkum     (501) staff       (20)       17 2024-05-27 12:27:34.000000 rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/top_level.txt
+drwxr-xr-x   0 humkum     (501) staff       (20)        0 2024-05-27 12:27:34.271658 rocketmq-client-python-mi-1.0.2/samples/
+-rw-r--r--   0 humkum     (501) staff       (20)        0 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/samples/__init__.py
+-rw-r--r--   0 humkum     (501) staff       (20)     1331 2024-05-27 12:24:10.000000 rocketmq-client-python-mi-1.0.2/samples/consumer.py
+-rw-r--r--   0 humkum     (501) staff       (20)     3648 2022-11-24 03:05:30.000000 rocketmq-client-python-mi-1.0.2/samples/producer.py
+-rw-r--r--   0 humkum     (501) staff       (20)      256 2024-05-27 12:27:34.272145 rocketmq-client-python-mi-1.0.2/setup.cfg
+-rwxr-xr-x   0 humkum     (501) staff       (20)     2948 2024-05-27 12:27:15.000000 rocketmq-client-python-mi-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rocketmq-client-python-mi-1.0.1/LICENSE` & `rocketmq-client-python-mi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketmq-client-python-mi-1.0.1/README.md` & `rocketmq-client-python-mi-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 rocketmq-client-python is a lightweight wrapper around [rocketmq-client-cpp](https://github.com/apache/rocketmq-client-cpp), so you need install 
 `librocketmq` first.
 
 #### Download by binary release.
 
 - debian
     ```bash
-        wget https://git.n.xiaomi.com/streaming/rocketmq-client-cpp/uploads/45ffa8c069174d3936e89258ce874140/rocketmq-client-cpp-2.2.0.amd64.deb
-        sudo dpkg -i rocketmq-client-cpp-2.2.0.amd64.deb
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/bd4e86d6c0ef4c65b4ef7014e8fe5c72/rocketmq-client-cpp-2.2.1.amd64.deb
+        sudo dpkg -i rocketmq-client-cpp-2.2.1.amd64.deb
     ```
 
+- centos
+    ```bash
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/1b6ac162c409ef0534eb08aa2096af1d/rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+        sudo rpm -ivh rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+    ```
 ## Installation
 
 ```bash
 pip install rocketmq-client-python-mi
 ```
 
 ## Usage
```

### Comparing `rocketmq-client-python-mi-1.0.1/rocketmq_client_python_mi.egg-info/PKG-INFO` & `rocketmq-client-python-mi-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketmq-client-python-mi
-Version: 1.0.1
+Version: 1.0.2
 Summary: RocketMQ Python Client
 Home-page: UNKNOWN
 Author: apache.rocketmq
 Author-email: dev@rocketmq.apache.org
 License: UNKNOWN
 Keywords: rocketmq
 Platform: UNKNOWN
@@ -39,18 +39,23 @@
 rocketmq-client-python is a lightweight wrapper around [rocketmq-client-cpp](https://github.com/apache/rocketmq-client-cpp), so you need install 
 `librocketmq` first.
 
 #### Download by binary release.
 
 - debian
     ```bash
-        wget https://git.n.xiaomi.com/streaming/rocketmq-client-cpp/uploads/45ffa8c069174d3936e89258ce874140/rocketmq-client-cpp-2.2.0.amd64.deb
-        sudo dpkg -i rocketmq-client-cpp-2.2.0.amd64.deb
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/bd4e86d6c0ef4c65b4ef7014e8fe5c72/rocketmq-client-cpp-2.2.1.amd64.deb
+        sudo dpkg -i rocketmq-client-cpp-2.2.1.amd64.deb
     ```
 
+- centos
+    ```bash
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/1b6ac162c409ef0534eb08aa2096af1d/rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+        sudo rpm -ivh rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+    ```
 ## Installation
 
 ```bash
 pip install rocketmq-client-python-mi
 ```
 
 ## Usage
```

### Comparing `rocketmq-client-python-mi-1.0.1/PKG-INFO` & `rocketmq-client-python-mi-1.0.2/rocketmq_client_python_mi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketmq-client-python-mi
-Version: 1.0.1
+Version: 1.0.2
 Summary: RocketMQ Python Client
 Home-page: UNKNOWN
 Author: apache.rocketmq
 Author-email: dev@rocketmq.apache.org
 License: UNKNOWN
 Keywords: rocketmq
 Platform: UNKNOWN
@@ -39,18 +39,23 @@
 rocketmq-client-python is a lightweight wrapper around [rocketmq-client-cpp](https://github.com/apache/rocketmq-client-cpp), so you need install 
 `librocketmq` first.
 
 #### Download by binary release.
 
 - debian
     ```bash
-        wget https://git.n.xiaomi.com/streaming/rocketmq-client-cpp/uploads/45ffa8c069174d3936e89258ce874140/rocketmq-client-cpp-2.2.0.amd64.deb
-        sudo dpkg -i rocketmq-client-cpp-2.2.0.amd64.deb
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/bd4e86d6c0ef4c65b4ef7014e8fe5c72/rocketmq-client-cpp-2.2.1.amd64.deb
+        sudo dpkg -i rocketmq-client-cpp-2.2.1.amd64.deb
     ```
 
+- centos
+    ```bash
+        wget https://git.n.xiaomi.com/hankunming/RMQ-CPP-Client-Package/uploads/1b6ac162c409ef0534eb08aa2096af1d/rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+        sudo rpm -ivh rocketmq-client-cpp-2.2.1-centos.x86_64.rpm
+    ```
 ## Installation
 
 ```bash
 pip install rocketmq-client-python-mi
 ```
 
 ## Usage
```

### Comparing `rocketmq-client-python-mi-1.0.1/rocketmq/__init__.py` & `rocketmq-client-python-mi-1.0.2/rocketmq/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketmq-client-python-mi-1.0.1/rocketmq/client.py` & `rocketmq-client-python-mi-1.0.2/rocketmq/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from .consts import MessageProperty
 
 __all__ = ['SendStatus', 'Message', 'ReceivedMessage', 'Producer', 'PushConsumer', 'TransactionMQProducer',
            'TransactionStatus', 'ConsumeStatus']
 
 PY2 = sys.version_info[0] == 2
 if PY2:
+    text_type = unicode
     binary_type = str
 else:
     text_type = str
     binary_type = bytes
 
 SendResult = namedtuple('SendResult', ['status', 'msg_id', 'offset'])
 
@@ -265,14 +266,17 @@
 
     def set_producer_language(self, language):
         ffi_check(dll.SetProducerLanguage(self._handle, _to_bytes(language)))
 
     def set_producer_log_path(self, path):
         ffi_check(dll.SetProducerLogPath(self._handle, _to_bytes(path)))
 
+    def set_producer_absolute_log_path(self, path):
+        ffi_check(dll.SetProducerAbsoluteLogPath(self._handle, _to_bytes(path)))
+
     def set_producer_log_file_num_and_size(self, file_num, file_size):
         ffi_check(dll.SetProducerLogFileNumAndSize(self._handle, file_num, file_size))
 
     def set_producer_log_level(self, level):
         ffi_check(dll.SetProducerLogLevel(self._handle, _CLogLevel(level)))
 
     def start(self):
@@ -461,14 +465,17 @@
 
     def set_consumer_language(self, language):
         ffi_check(dll.SetPushConsumerLanguage(self._handle, _to_bytes(language)))
 
     def set_consumer_log_path(self, log_path):
         ffi_check(dll.SetPushConsumerLogPath(self._handle, _to_bytes(log_path)))
 
+    def set_consumer_absolute_log_path(self, log_path):
+        ffi_check(dll.SetPushConsumerAbsoluteLogPath(self._handle, _to_bytes(log_path)))
+
     def set_consume_from_where(self, consume_from_where):
         ffi_check(dll.SetPushConsumerConsumeFromWhere(self._handle, consume_from_where))
 
     def set_consumer_log_file_num_and_size(self, file_num, file_size):
         ffi_check(dll.SetPushConsumerLogFileNumAndSize(self._handle, file_num, file_size))
 
     def set_consumer_log_level(self, level):
```

### Comparing `rocketmq-client-python-mi-1.0.1/rocketmq/ffi.py` & `rocketmq-client-python-mi-1.0.2/rocketmq/ffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,26 @@
     MALLOC_FAILED = 2
     # producer
     PRODUCER_START_FAILED = 10
     PRODUCER_SEND_SYNC_FAILED = 11
     PRODUCER_SEND_ONEWAY_FAILED = 12
     PRODUCER_SEND_ORDERLY_FAILED = 13
     PRODUCER_SEND_ASYNC_FAILED = 14
+    PRODUCER_SEND_ORDERLYASYNC_FAILED = 15
+    PRODUCER_SEND_TRANSACTION_FAILED = 16
     # push consumer
+    PUSH_CONSUMER_ERROR_CODE_START = 20
     PUSH_CONSUMER_START_FAILED = 20
+    # pull consumer
+    PULL_CONSUMER_ERROR_CODE_START = 30
+    PULL_CONSUMER_START_FAILED = 30
+    PULL_CONSUMER_FETCH_MQ_FAILED = 31
+    PULL_CONSUMER_FETCH_MESSAGE_FAILED = 32
+
+    Not_Support = 500
 
     NOT_SUPPORT_NOW = -1
 
 
 class _CLogLevel(CtypesEnum):
     FATAL = 1
     ERROR = 2
@@ -223,16 +233,26 @@
 
 dll.CreateTransactionProducer.argtypes = [c_char_p, TRANSACTION_CHECK_CALLBACK, c_void_p]
 dll.CreateTransactionProducer.restype = c_void_p
 
 dll.SendMessageTransaction.argtypes = [c_void_p, c_void_p, LOCAL_TRANSACTION_EXECUTE_CALLBACK, c_void_p,
                                        POINTER(_CSendResult)]
 dll.SendMessageTransaction.restype = c_int
+dll.SetProducerMessageTrace.argtypes = [c_void_p, _CTraceModel]
+dll.SetProducerMessageTrace.restype = c_int
 dll.SetProducerLanguage.argtypes = [c_void_p, c_char_p]
 dll.SetProducerLanguage.restype = c_int
+dll.SetProducerLogPath.argtypes = [c_void_p, c_char_p]
+dll.SetProducerLogPath.restype = c_int
+dll.SetProducerAbsoluteLogPath.argtypes = [c_void_p, c_char_p]
+dll.SetProducerAbsoluteLogPath.restype = c_int
+dll.SetProducerLogFileNumAndSize.argtypes = [c_void_p, c_int, c_long]
+dll.SetProducerLogFileNumAndSize.restype = c_int
+dll.SetProducerLogLevel.argtypes = [c_void_p, _CLogLevel]
+dll.SetProducerLogLevel.restype = c_int
 
 # Push Consumer
 MSG_CALLBACK_FUNC = ctypes.CFUNCTYPE(c_int, c_void_p, c_void_p)
 dll.CreatePushConsumer.argtypes = [c_char_p]
 dll.CreatePushConsumer.restype = c_void_p
 dll.DestroyPushConsumer.argtypes = [c_void_p]
 dll.DestroyPushConsumer.restype = _CStatus
@@ -270,17 +290,25 @@
 dll.SetPushConsumerLogPath.restype = _CStatus
 dll.SetPushConsumerLogFileNumAndSize.argtypes = [c_void_p, c_int, c_long]
 dll.SetPushConsumerLogFileNumAndSize.restype = _CStatus
 dll.SetPushConsumerLogLevel.argtypes = [c_void_p, _CLogLevel]
 dll.SetPushConsumerLogLevel.restype = _CStatus
 dll.SetPushConsumerMessageModel.argtypes = [c_void_p, MessageModel]
 dll.SetPushConsumerMessageModel.restype = _CStatus
+dll.SetPushConsumerMessageTrace.argtypes = [c_void_p, _CTraceModel]
+dll.SetPushConsumerMessageTrace.restype = c_int
 dll.SetPushConsumerLanguage.argtypes = [c_void_p, c_char_p]
 dll.SetPushConsumerLanguage.restype = c_int
+dll.SetPushConsumerLogPath.argtypes = [c_void_p, c_char_p]
+dll.SetPushConsumerLogPath.restype = c_int
+dll.SetPushConsumerAbsoluteLogPath.argtypes = [c_void_p, c_char_p]
+dll.SetPushConsumerAbsoluteLogPath.restype = c_int
 dll.SetPushConsumerConsumeFromWhere.argtypes = [c_void_p, _CConsumeFromWhere]
 dll.SetPushConsumerConsumeFromWhere.restype = _CStatus
-dll.SetPushConsumerMessageTrace.argtypes = [c_void_p, _CTraceModel]
-dll.SetPushConsumerMessageTrace.restype = c_int
+dll.SetPushConsumerLogFileNumAndSize.argtypes = [c_void_p, c_int, c_long]
+dll.SetPushConsumerLogFileNumAndSize.restype = c_int
+dll.SetPushConsumerLogLevel.argtypes = [c_void_p, _CLogLevel]
+dll.SetPushConsumerLogLevel.restype = c_int
 
 # Misc
 dll.GetLatestErrorMessage.argtypes = []
 dll.GetLatestErrorMessage.restype = c_char_p
```

### Comparing `rocketmq-client-python-mi-1.0.1/rocketmq/consts.py` & `rocketmq-client-python-mi-1.0.2/rocketmq/consts.py`

 * *Files identical despite different names*

### Comparing `rocketmq-client-python-mi-1.0.1/setup.py` & `rocketmq-client-python-mi-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.install_lib = self.install_platlib
 
 
 cmdclass['install'] = InstallPlatlib
 
 setup(
     name='rocketmq-client-python-mi',
-    version='1.0.1',
+    version='1.0.2',
     author='apache.rocketmq',
     author_email='dev@rocketmq.apache.org',
     packages=find_packages(exclude=('tests', 'tests.*')),
     keywords='rocketmq',
     description='RocketMQ Python Client',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `rocketmq-client-python-mi-1.0.1/samples/consumer.py` & `rocketmq-client-python-mi-1.0.2/samples/consumer.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,25 +16,21 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from rocketmq.client import PushConsumer, ConsumeStatus
 import time
 
-from rocketmq.ffi import _CConsumeFromWhere
-
-
 def callback(msg):
     print(msg.id, msg.body,  msg.get_property('property'))
     return ConsumeStatus.CONSUME_SUCCESS
 
 def start_consume_message():
     consumer = PushConsumer('consumer_group')
     consumer.set_name_server_address('127.0.0.1:9876')
-    consumer.set_consume_from_where(_CConsumeFromWhere.CONSUME_FROM_LAST_OFFSET)
     consumer.subscribe('TopicTest', callback)
     print ('start consume message')
     consumer.start()
 
     while True:
         time.sleep(3600)
```

### Comparing `rocketmq-client-python-mi-1.0.1/samples/producer.py` & `rocketmq-client-python-mi-1.0.2/samples/producer.py`

 * *Files identical despite different names*

