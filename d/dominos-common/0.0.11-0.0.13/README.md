# Comparing `tmp/dominos_common-0.0.11.tar.gz` & `tmp/dominos_common-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominos_common-0.0.11.tar", last modified: Wed May 22 17:24:03 2024, max compression
+gzip compressed data, was "dominos_common-0.0.13.tar", last modified: Mon May 27 07:18:49 2024, max compression
```

## Comparing `dominos_common-0.0.11.tar` & `dominos_common-0.0.13.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.669839 dominos_common-0.0.11/
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      676 2024-05-22 17:24:03.669580 dominos_common-0.0.11/PKG-INFO
--rw-r--r--   0 dqlbyzy    (501) staff       (20)       17 2024-05-22 16:24:32.000000 dominos_common-0.0.11/README.md
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.666721 dominos_common-0.0.11/app/
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.667449 dominos_common-0.0.11/app/dominos_common/
--rw-r--r--   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 16:54:22.000000 dominos_common-0.0.11/app/dominos_common/__init__.py
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.668150 dominos_common-0.0.11/app/dominos_common/src/
--rw-r--r--   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 16:48:07.000000 dominos_common-0.0.11/app/dominos_common/src/__init__.py
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.668948 dominos_common-0.0.11/app/dominos_common/src/db_helper/
--rw-r--r--   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 16:45:21.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/__init__.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      524 2024-05-22 16:54:29.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/address_model.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      615 2024-05-22 16:58:14.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/database.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)     1100 2024-05-22 17:22:27.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/item_model.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)     1489 2024-05-22 17:23:43.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/order_model.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      454 2024-05-22 17:23:52.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/restaurant_model.py
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      706 2024-05-22 17:23:55.000000 dominos_common-0.0.11/app/dominos_common/src/db_helper/user_model.py
-drwxr-xr-x   0 dqlbyzy    (501) staff       (20)        0 2024-05-22 17:24:03.669128 dominos_common-0.0.11/app/dominos_common.egg-info/
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      676 2024-05-22 17:24:03.000000 dominos_common-0.0.11/app/dominos_common.egg-info/PKG-INFO
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      628 2024-05-22 17:24:03.000000 dominos_common-0.0.11/app/dominos_common.egg-info/SOURCES.txt
--rw-r--r--   0 dqlbyzy    (501) staff       (20)        1 2024-05-22 17:24:03.000000 dominos_common-0.0.11/app/dominos_common.egg-info/dependency_links.txt
--rw-r--r--   0 dqlbyzy    (501) staff       (20)       87 2024-05-22 17:24:03.000000 dominos_common-0.0.11/app/dominos_common.egg-info/requires.txt
--rw-r--r--   0 dqlbyzy    (501) staff       (20)       15 2024-05-22 17:24:03.000000 dominos_common-0.0.11/app/dominos_common.egg-info/top_level.txt
--rw-r--r--   0 dqlbyzy    (501) staff       (20)       38 2024-05-22 17:24:03.669886 dominos_common-0.0.11/setup.cfg
--rw-r--r--   0 dqlbyzy    (501) staff       (20)      908 2024-05-22 17:22:02.000000 dominos_common-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 07:18:49.862089 dominos_common-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:18:45.000000 dominos_common-0.0.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/app/dominos_common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/app/dominos_common/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/app/dominos_common/src/db_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/item_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/order_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/restaurant_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-27 07:18:45.000000 dominos_common-0.0.13/app/dominos_common/src/db_helper/user_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:18:49.862089 dominos_common-0.0.13/app/dominos_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 07:18:49.000000 dominos_common-0.0.13/app/dominos_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-27 07:18:49.000000 dominos_common-0.0.13/app/dominos_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:18:49.000000 dominos_common-0.0.13/app/dominos_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 07:18:49.000000 dominos_common-0.0.13/app/dominos_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 07:18:49.000000 dominos_common-0.0.13/app/dominos_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:18:49.862089 dominos_common-0.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-27 07:18:45.000000 dominos_common-0.0.13/setup.py
```

### Comparing `dominos_common-0.0.11/PKG-INFO` & `dominos_common-0.0.13/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominos_common
-Version: 0.0.11
+Version: 0.0.13
 Summary: Share utilities and models across the Dominos app
 Home-page: https://github.com/dekelbyz/dominos-common
 Author: Dekel Bayazi
 Author-email: bayazi455@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -14,8 +14,8 @@
 Requires-Dist: bson>=0.5.10
 Requires-Dist: SQLAlchemy>=2.0.30
 Requires-Dist: psycopg2-binary>=2.9.9
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
-# Hello README
+# dominos-common
```

### Comparing `dominos_common-0.0.11/app/dominos_common/src/db_helper/address_model.py` & `dominos_common-0.0.13/app/dominos_common/src/db_helper/address_model.py`

 * *Files identical despite different names*

### Comparing `dominos_common-0.0.11/app/dominos_common/src/db_helper/database.py` & `dominos_common-0.0.13/app/dominos_common/src/db_helper/database.py`

 * *Files identical despite different names*

### Comparing `dominos_common-0.0.11/app/dominos_common/src/db_helper/item_model.py` & `dominos_common-0.0.13/app/dominos_common/src/db_helper/item_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     price: Mapped[int] = Column(Float(), nullable=False)
 
 
 class ItemOptionGroup(Base):
     __tablename__ = 'item_option_groups'
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
     name = Column(String(50), unique=True, nullable=False)
-    item_id = mapped_column(ForeignKey('items.id'), nullable=False)
+    item_id = mapped_column(ForeignKey(Item.id), nullable=False)
     multiple_choice = Column(Boolean(), nullable=False, default=False)
 
 
 class ItemOption(Base):
     __tablename__ = 'item_options'
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
     name = Column(String(50), unique=True, nullable=False)
     item_option_group_id = mapped_column(
-        ForeignKey('item_option_groups.id'), nullable=False)
+        ForeignKey(ItemOptionGroup.id), nullable=False)
     price = Column(Float(), nullable=False)
```

### Comparing `dominos_common-0.0.11/app/dominos_common/src/db_helper/order_model.py` & `dominos_common-0.0.13/app/dominos_common/src/db_helper/order_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy import ForeignKey, Enum, Column, Integer, Float
 from typing import List
 from enum import Enum as PyEnum
 from .item_model import Item
 from .database import Base
 
+from .user_model import User
+from .restaurant_model import Restaurant
+from .address_model import Address
+from .item_model import Item
 
 class OrderStatusEnum(PyEnum):
     PENDING = 'pending'
     ACCEPTED = 'accepted'
     IN_PROGRESS = 'in_progress'
     READY = 'ready'
     DELIVERY = 'delivery'
@@ -22,22 +26,22 @@
     id = Column(Integer, primary_key=True, autoincrement=True)
     value = Column(Enum(OrderStatusEnum))
 
 
 class Order(Base):
     __tablename__ = 'orders'
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    order_status = mapped_column(ForeignKey('order_status.id'))
+    order_status = mapped_column(ForeignKey(OrderStatus.id))
     items: Mapped[List['OrderItem']] = relationship()
-    branch_id = mapped_column(ForeignKey('restaurants.id'), nullable=False)
-    address_id = mapped_column(ForeignKey('addresses.id'), nullable=False)
-    customer_id = mapped_column(ForeignKey('users.id'), nullable=False)
+    branch_id = mapped_column(ForeignKey(Restaurant.id), nullable=False)
+    address_id = mapped_column(ForeignKey(Address.id), nullable=False)
+    customer_id = mapped_column(ForeignKey(User.id), nullable=False)
     total_price = Column(Float())
 
 
 class OrderItem(Base):
     __tablename__ = 'order_items'
     id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    item_id = mapped_column(ForeignKey('items.id'), nullable=False)
+    item_id = mapped_column(ForeignKey(Item.id), nullable=False)
     item_details: Mapped[Item] = relationship()
-    order_id = mapped_column(ForeignKey('orders.id'), nullable=False)
+    order_id = mapped_column(ForeignKey(Order.id), nullable=False)
     quantity = Column(Integer(), nullable=False)
```

### Comparing `dominos_common-0.0.11/app/dominos_common/src/db_helper/user_model.py` & `dominos_common-0.0.13/app/dominos_common/src/db_helper/user_model.py`

 * *Files identical despite different names*

### Comparing `dominos_common-0.0.11/app/dominos_common.egg-info/PKG-INFO` & `dominos_common-0.0.13/app/dominos_common.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominos_common
-Version: 0.0.11
+Version: 0.0.13
 Summary: Share utilities and models across the Dominos app
 Home-page: https://github.com/dekelbyz/dominos-common
 Author: Dekel Bayazi
 Author-email: bayazi455@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -14,8 +14,8 @@
 Requires-Dist: bson>=0.5.10
 Requires-Dist: SQLAlchemy>=2.0.30
 Requires-Dist: psycopg2-binary>=2.9.9
 Provides-Extra: dev
 Requires-Dist: pytest>=7.0; extra == "dev"
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
-# Hello README
+# dominos-common
```

### Comparing `dominos_common-0.0.11/app/dominos_common.egg-info/SOURCES.txt` & `dominos_common-0.0.13/app/dominos_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dominos_common-0.0.11/setup.py` & `dominos_common-0.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
-with open("app/README.md", "r") as f:
+with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="dominos_common",
-    version="0.0.11",
+    version="0.0.13",
     description="Share utilities and models across the Dominos app",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dekelbyz/dominos-common",
     author="Dekel Bayazi",
```

