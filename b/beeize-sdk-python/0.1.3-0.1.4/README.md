# Comparing `tmp/beeize-sdk-python-0.1.3.tar.gz` & `tmp/beeize-sdk-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beeize-sdk-python-0.1.3.tar", last modified: Mon Apr 29 14:40:35 2024, max compression
+gzip compressed data, was "beeize-sdk-python-0.1.4.tar", last modified: Mon May 27 01:08:12 2024, max compression
```

## Comparing `beeize-sdk-python-0.1.3.tar` & `beeize-sdk-python-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.187725 beeize-sdk-python-0.1.3/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-29 14:40:35.187369 beeize-sdk-python-0.1.3/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)     6405 2024-04-08 15:33:34.000000 beeize-sdk-python-0.1.3/README.md
--rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-04-29 14:40:35.187834 beeize-sdk-python-0.1.3/setup.cfg
--rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2024-04-29 14:40:25.000000 beeize-sdk-python-0.1.3/setup.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.178949 beeize-sdk-python-0.1.3/src/
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.182767 beeize-sdk-python-0.1.3/src/beeize/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       14 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1130 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/config.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.3/src/beeize/consts.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     1571 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/scraper.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.185769 beeize-sdk-python-0.1.3/src/beeize/storages/
--rw-r--r--   0 zhaoyang   (501) staff       (20)      176 2024-04-27 11:34:11.000000 beeize-sdk-python-0.1.3/src/beeize/storages/__init__.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2846 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.3/src/beeize/storages/dataset.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     6530 2024-04-29 14:39:49.000000 beeize-sdk-python-0.1.3/src/beeize/storages/kv_store.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     5203 2024-04-27 11:41:19.000000 beeize-sdk-python-0.1.3/src/beeize/storages/request_queue.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)        0 2023-11-15 15:27:00.000000 beeize-sdk-python-0.1.3/src/beeize/storages/storage_manager.py
--rw-r--r--   0 zhaoyang   (501) staff       (20)     2174 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.3/src/beeize/utils.py
-drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-04-29 14:40:35.186961 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/
--rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyang   (501) staff       (20)      476 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-04-29 14:40:35.000000 beeize-sdk-python-0.1.3/src/beeize_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-05-27 01:08:12.651242 beeize-sdk-python-0.1.4/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-05-27 01:08:12.650948 beeize-sdk-python-0.1.4/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6405 2024-04-08 15:33:34.000000 beeize-sdk-python-0.1.4/README.md
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       38 2024-05-27 01:08:12.651334 beeize-sdk-python-0.1.4/setup.cfg
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      364 2024-05-26 12:16:20.000000 beeize-sdk-python-0.1.4/setup.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-05-27 01:08:12.642467 beeize-sdk-python-0.1.4/src/
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-05-27 01:08:12.646236 beeize-sdk-python-0.1.4/src/beeize/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       14 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.4/src/beeize/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2216 2024-05-27 01:07:42.000000 beeize-sdk-python-0.1.4/src/beeize/config.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      132 2023-12-03 06:12:45.000000 beeize-sdk-python-0.1.4/src/beeize/consts.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     1585 2024-05-26 11:56:39.000000 beeize-sdk-python-0.1.4/src/beeize/scraper.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-05-27 01:08:12.648972 beeize-sdk-python-0.1.4/src/beeize/storages/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      176 2024-04-27 11:34:11.000000 beeize-sdk-python-0.1.4/src/beeize/storages/__init__.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2504 2024-05-26 12:24:36.000000 beeize-sdk-python-0.1.4/src/beeize/storages/dataset.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     6528 2024-05-26 11:56:39.000000 beeize-sdk-python-0.1.4/src/beeize/storages/kv_store.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     5201 2024-05-26 11:56:39.000000 beeize-sdk-python-0.1.4/src/beeize/storages/request_queue.py
+-rw-r--r--   0 zhaoyang   (501) staff       (20)     2174 2024-04-27 11:35:18.000000 beeize-sdk-python-0.1.4/src/beeize/utils.py
+drwxr-xr-x   0 zhaoyang   (501) staff       (20)        0 2024-05-27 01:08:12.650579 beeize-sdk-python-0.1.4/src/beeize_sdk_python.egg-info/
+-rw-r--r--   0 zhaoyang   (501) staff       (20)       97 2024-05-27 01:08:12.000000 beeize-sdk-python-0.1.4/src/beeize_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyang   (501) staff       (20)      437 2024-05-27 01:08:12.000000 beeize-sdk-python-0.1.4/src/beeize_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        1 2024-05-27 01:08:12.000000 beeize-sdk-python-0.1.4/src/beeize_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyang   (501) staff       (20)        7 2024-05-27 01:08:12.000000 beeize-sdk-python-0.1.4/src/beeize_sdk_python.egg-info/top_level.txt
```

### Comparing `beeize-sdk-python-0.1.3/README.md` & `beeize-sdk-python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `beeize-sdk-python-0.1.3/src/beeize/scraper.py` & `beeize-sdk-python-0.1.4/src/beeize/scraper.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 
 from .config import Configuration
 from .storages import Dataset, RequestQueue, KeyValueStore
 
 
 class Scraper:
     _default_instance: Optional['Scraper'] = None
-    _config: Configuration
+    config: Configuration
 
     def __init__(self, config: Optional[Configuration] = None) -> None:
-        self._config: Configuration = config or Configuration()
-        self.dataset = Dataset(None, config=self._config)
-        self.request_queue = RequestQueue(id=None, config=self._config)
-        self.key_value_store = KeyValueStore(id=None, config=self._config)
+        self.config: Configuration = config or Configuration()
+        self.dataset = Dataset(None, config=self.config)
+        self.request_queue = RequestQueue(id=None, config=self.config)
+        self.key_value_store = KeyValueStore(id=None, config=self.config)
 
     def push_data(self, data: Any) -> None:
         if not data:
             return
         self.dataset.push_data(data)
 
 
 if __name__ == '__main__':
     # python -m src.beeize.scraper
     scraper = Scraper()
+    scraper.config
     """ 存储数据
     scraper.push_data({"key": "dafwew "})
     """
 
     """ 添加请求"""
     request_queue = scraper.request_queue
     item = request_queue.add_request(
```

### Comparing `beeize-sdk-python-0.1.3/src/beeize/storages/dataset.py` & `beeize-sdk-python-0.1.4/src/beeize/storages/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 
 class Dataset:
     _lock = threading.Lock()
 
     def __init__(self, id: [None, str], config: Configuration):
         self._id = id or config.get_config_value('DATASET_ID', 'default')
-        self._config = config
+        self.config = config
         self.datasets_path = os.path.join(
-            self._config.base_dir,
+            self.config.base_dir,
             'datasets',
             self._id
         )
         os.makedirs(self.datasets_path, exist_ok=True)
         self.metadata = self.load_metadata()
 
     def load_metadata(self):
@@ -46,25 +46,19 @@
 
     def push_data(self, data: Any) -> None:
         if not isinstance(data, (dict, list, str, int, float, bool, type(None))):
             raise ValueError("Data is not JSON serializable")
 
         with self._lock:
             try:
-                next_file_number = self.get_next_file_number_with_lock()
-                file_name = f"{str(next_file_number).zfill(9)}.json"
+                self.metadata['itemCount'] += 1
+                file_name = f"{str(self.metadata['itemCount']).zfill(9)}.json"
                 file_path = os.path.join(self.datasets_path, file_name)
                 with open(file_path, 'w', encoding='utf-8', errors='ignore') as file:
                     json.dump(data, file, indent=4, ensure_ascii=False)
                     file.flush()
                     os.fsync(file.fileno())
-                self.metadata['itemCount'] += 1
                 self.metadata['accessedAt'] = datetime.now(timezone.utc).isoformat()
                 self.metadata['modifiedAt'] = datetime.now(timezone.utc).isoformat()
                 self.update_metadata()  # 保存元数据更改
             except IOError as e:
                 print(f"An error occurred: {e}")
-
-    def get_next_file_number_with_lock(self) -> int:
-        files = [f for f in os.listdir(self.datasets_path) if f.endswith('.json') and not f.startswith('__')]
-        numbers = sorted([int(f.split('.')[0]) for f in files])
-        return numbers[-1] + 1 if numbers else 1
```

### Comparing `beeize-sdk-python-0.1.3/src/beeize/storages/kv_store.py` & `beeize-sdk-python-0.1.4/src/beeize/storages/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 
 class KeyValueStore:
     _lock = threading.Lock()
 
     def __init__(self, id: [None, str], config: Configuration):
         self._id = id or config.get_config_value('KV_STORE_ID', 'default')
-        self._config = config
+        self.config = config
         self.kv_store_path = os.path.join(
-            self._config.base_dir,
+            self.config.base_dir,
             'kv_stores',
             self._id
         )
         os.makedirs(self.kv_store_path, exist_ok=True)
         self.metadata = self.load_metadata()
 
     def load_metadata(self):
```

### Comparing `beeize-sdk-python-0.1.3/src/beeize/storages/request_queue.py` & `beeize-sdk-python-0.1.4/src/beeize/storages/request_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from ..config import Configuration
 from ..utils import _unique_key_to_request_id
 
 
 class RequestQueue:
     def __init__(self, id: [None, str], config: Configuration):
         self._id = id or config.get_config_value('REQUEST_QUEUE_ID', 'default')
-        self._config = config
+        self.config = config
         self._lock = threading.Lock()
         self.request_queues_path = os.path.join(
-            self._config.base_dir,
+            self.config.base_dir,
             'request_queues',
             self._id
         )
         os.makedirs(self.request_queues_path, exist_ok=True)
         self._queue = []
         self._requests_cache = {}
         self._handled_count = 0
```

### Comparing `beeize-sdk-python-0.1.3/src/beeize/utils.py` & `beeize-sdk-python-0.1.4/src/beeize/utils.py`

 * *Files identical despite different names*

