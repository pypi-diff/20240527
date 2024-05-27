# Comparing `tmp/popoll_backend-0.0.56.tar.gz` & `tmp/popoll_backend-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.56.tar", last modified: Tue May 21 14:08:51 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.57.tar", last modified: Mon May 27 08:53:21 2024, max compression
```

## Comparing `popoll_backend-0.0.56.tar` & `popoll_backend-0.0.57.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.707959 popoll_backend-0.0.56/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-21 14:08:51.706959 popoll_backend-0.0.56/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.690958 popoll_backend-0.0.56/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.692958 popoll_backend-0.0.56/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.693958 popoll_backend-0.0.56/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.696958 popoll_backend-0.0.56/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/date_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/dates_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/instrument_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/instruments_payload.py
--rw-rw-rw-   0 root         (0) root         (0)     1288 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/user.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/user_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/users_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.701959 popoll_backend-0.0.56/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     2214 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     1470 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/delete_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.706959 popoll_backend-0.0.56/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-21 14:08:51.000000 popoll_backend-0.0.56/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2715 2024-05-21 14:08:51.000000 popoll_backend-0.0.56/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:08:51.000000 popoll_backend-0.0.56/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-21 14:08:51.000000 popoll_backend-0.0.56/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-21 14:08:51.000000 popoll_backend-0.0.56/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-21 14:08:45.000000 popoll_backend-0.0.56/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 14:08:51.707959 popoll_backend-0.0.56/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:08:51.706959 popoll_backend-0.0.56/tests/
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_01_db_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_02_simple_adds.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_03_no_duplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_04_update_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_05_update_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_06_update_answer_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_07_delete_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_08_delete_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_09_delete_user_date_entries.py
--rw-rw-rw-   0 root         (0) root         (0)     1378 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_10_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_11_get_users_sort_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_12_get_dates_sort_dateTime.py
--rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_13_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_14_get_answers_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_15_multi_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_16_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_17_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_19_delete_database.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_20_add_answer_no_dupe.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_21_get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_22_add_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     1174 2024-05-21 14:08:31.000000 popoll_backend-0.0.56/tests/test_23_get_instruments_with_is_used.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.936738 popoll_backend-0.0.57/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     7908 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.938738 popoll_backend-0.0.57/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.939738 popoll_backend-0.0.57/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.942738 popoll_backend-0.0.57/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/empty.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.948738 popoll_backend-0.0.57/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     2226 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1860 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_all_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_date_details.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1028 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_user_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_user_with_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.953738 popoll_backend-0.0.57/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-27 08:53:21.000000 popoll_backend-0.0.57/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-27 08:53:16.000000 popoll_backend-0.0.57/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 08:53:21.954738 popoll_backend-0.0.57/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:53:21.952738 popoll_backend-0.0.57/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_01_get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_02_create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_03_update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_04_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_08_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_09_create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_10_get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_11_update_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_12_delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_13_get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_14_create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_15_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_16_update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_17_delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_18_create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_19_update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_20_delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_21_get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_22_get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-27 08:53:01.000000 popoll_backend-0.0.57/tests/test_23_get_create_session.py
```

### Comparing `popoll_backend-0.0.56/PKG-INFO` & `popoll_backend-0.0.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.56
+Version: 0.0.57
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.56/popoll_backend/__main__.py` & `popoll_backend-0.0.57/popoll_backend/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,40 +18,48 @@
 from popoll_backend.query.create_instrument import CreateInstrument
 from popoll_backend.query.create_poll import CreatePoll
 from popoll_backend.query.create_user import CreateUser
 from popoll_backend.query.delete_answer import DeleteAnswer
 from popoll_backend.query.delete_date import DeleteDate
 from popoll_backend.query.delete_instrument import DeleteInstrument
 from popoll_backend.query.delete_user import DeleteUser
+from popoll_backend.query.get_all_instruments import GetAllInstruments
+from popoll_backend.query.get_answer import GetAnswer
 from popoll_backend.query.get_date import GetDate
+from popoll_backend.query.get_date_details import GetDateDetails
 from popoll_backend.query.get_dates import GetDates
 from popoll_backend.query.get_instrument import GetInstrument
 from popoll_backend.query.get_instruments import GetInstruments
 from popoll_backend.query.get_poll import GetPoll
 from popoll_backend.query.get_search_answer import GetSearchAnswer
 from popoll_backend.query.get_session import GetSession
-from popoll_backend.query.get_user import GetUser
+from popoll_backend.query.get_user_details import GetUserDetails
+from popoll_backend.query.get_user_with_instruments import GetUserWithInstruments
 from popoll_backend.query.get_users import GetUsers
 from popoll_backend.query.update_answer import UpdateAnswer
 from popoll_backend.query.update_date import UpdateDate
 from popoll_backend.query.update_poll import UpdatePoll
 from popoll_backend.query.create_session import CreateSession
 from popoll_backend.query.update_user import UpdateUser
 
 
 app = flask.Flask(__name__)
 CORS(app)
 api = Api(app)
 
 
 def body(request: flask.request, param: str, default: Any=None, mandatory=True):
-    _body = json.loads(request.data)
-    return _body[param] if mandatory else _body.get(param, default)
-
+    if request.data != None:
+        _body = json.loads(request.data)
+        return _body[param] if mandatory else _body.get(param, default)
+    else:
+        return flask.abort(400, f'Missing parameter [{param}]') if mandatory else default
 
+def queryParam(request: flask.request, param: str) -> bool:
+    return request.args.get(param, '') == 'true'
 
 def history(f):
     @wraps(f)
     def decorated(*args, **kwargs):
         _poll = kwargs.get('poll')
         res = f(*args, **kwargs)
         os.makedirs(os.path.join('.history', _poll), exist_ok=True)
@@ -60,118 +68,122 @@
         handler = logging.handlers.RotatingFileHandler(os.path.join('.history', _poll, f'{_poll}.history.log'), maxBytes=1024*1024, backupCount=10)
         logger.addHandler(handler)
         logger.warning(json.dumps(History(flask.request, res, kwargs).toJSON()))
         return res
     return decorated
 
 
+
+
+
 class PollEndpoint(Resource):
-    def get(self, poll: str): return GetPoll(poll).run()
+    def get(self, poll: str) -> str: return GetPoll(poll).run().toJSON()
     
     @history
-    def post(self, poll:str): return CreatePoll(poll, body(flask.request, 'name', mandatory=False, default=poll), body(flask.request, 'instruments', mandatory=False, default=[]), body(flask.request, 'color', mandatory=False, default="#000000")).run()
+    def post(self, poll:str) -> str: return CreatePoll(poll, body(flask.request, 'name', mandatory=False, default=poll), body(flask.request, 'instruments', mandatory=False, default=[]), body(flask.request, 'color', mandatory=False, default="#000000")).run().toJSON()
     
     @history
-    def put(self, poll:str): return UpdatePoll(poll, body(flask.request, 'name'), body(flask.request, 'color')).run()
-    
-    
+    def put(self, poll:str) -> str: return UpdatePoll(poll, body(flask.request, 'name'), body(flask.request, 'color')).run().toJSON()
     
     
     
 
 class InstrumentsEndpoint(Resource):
-    def get(self, poll: str) -> Dict[str, Any]: return GetInstruments(poll).run()
+    def get(self, poll: str) -> str: 
+        if queryParam(flask.request, 'used_only'):
+            return GetInstruments(poll).run().toJSON()
+        else:
+            return GetAllInstruments(poll).run().toJSON()
     
-    @history
-    def post(self, poll: str) -> int: 
-        return CreateInstrument(poll, body(flask.request, 'name'), body(flask.request, 'rank')).run()
-    
-    
-class InstrumentEndpoint(Resource):
-    def get(self, poll: str, id: int) -> Dict[str, Any]: return GetInstrument(poll, id).run()
     
-    @history
-    def delete(self, poll: str, id: int):
-        return DeleteInstrument(poll, id).run()
-
 
 
 
 
 
 
 class UsersEndpoint(Resource):
-    def get(self, poll: str) -> Dict[str, Any]: return GetUsers(poll, details=True).run()
+    def get(self, poll: str) -> str: return GetUsers(poll).run().toJSON()
     
     @history
-    def post(self, poll: str) -> int: return CreateUser(poll, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run()
+    def post(self, poll: str) -> str: return CreateUser(poll, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
 
 
 
 class UserEndpoint(Resource):
-    def get(self, poll: str, id:int) -> Dict[str, Any]: return GetUser(poll, id, details=True).run()
+    def get(self, poll: str, id:int) -> str: 
+        if queryParam(flask.request, 'details'):
+            return GetUserDetails(poll, id).run().toJSON()
+        else:
+            return GetUserWithInstruments(poll, id).run().toJSON()
     
     @history
-    def put(self, poll: str, id: int) -> int: return UpdateUser(poll, id, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run()
+    def put(self, poll: str, id: int) -> str: return UpdateUser(poll, id, body(flask.request, 'user')['name'], body(flask.request, 'main_instrument')['id'], [i['id'] for i in body(flask.request, 'instruments')]).run().toJSON()
     
     @history
-    def delete(self, poll: str, id: int) -> int: return DeleteUser(poll, id).run()
+    def delete(self, poll: str, id: int) -> str: return DeleteUser(poll, id).run().toJSON()
 
 
 
 
 
 
 
 class DatesEndpoint(Resource):
-    def get(self, poll: str): return GetDates(poll).run()
+    def get(self, poll: str) -> str: return GetDates(poll).run().toJSON()
     
     @history
-    def post(self, poll: str) -> int: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run()
+    def post(self, poll: str) -> str: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run().toJSON()
 
 
 
 class DateEndpoint(Resource):
-    def get(self, poll: str, id:int) -> Dict[str, Any]: return GetDate(poll, id, details=True).run()
+    def get(self, poll: str, id:int) -> str:
+        if queryParam(flask.request, 'details'):
+            return GetDateDetails(poll, id).run().toJSON()
+        else:
+            return GetDate(poll, id).run().toJSON()
     
     @history
-    def put(self, poll: str, id: int) -> int: return UpdateDate(poll, id, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run()
+    def put(self, poll: str, id: int) -> str: return UpdateDate(poll, id, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run().toJSON()
     
     @history
-    def delete(self, poll: str, id: int) -> int: return DeleteDate(poll, id).run()
+    def delete(self, poll: str, id: int) -> str: return DeleteDate(poll, id).run().toJSON()
 
 
 
 
 
 
 
 class AnswersEndpoint(Resource):
     
     @history
-    def post(self, poll: str) -> int: return CreateAnswer(poll, body(flask.request, 'user_id'), body(flask.request, 'date_id')).run()
+    def post(self, poll: str) -> str: return CreateAnswer(poll, body(flask.request, 'user_id'), body(flask.request, 'date_id')).run().toJSON()
 
 
 class AnswerEndpoint(Resource):
     
+    def get(self, poll: str, id:int) -> str: return GetAnswer(poll, id).run().toJSON()
+    
     @history
-    def put(self, poll: str, id: int) -> int: return UpdateAnswer(poll, id, body(flask.request, 'response')).run()
+    def put(self, poll: str, id: int) -> str: return UpdateAnswer(poll, id, body(flask.request, 'response')).run().toJSON()
     
     @history
-    def delete(self, poll: str, id: int) -> int: return DeleteAnswer(poll, id).run()
+    def delete(self, poll: str, id: int) -> str: return DeleteAnswer(poll, id).run().toJSON()
 
 class GetAnswerEndpoint(Resource):
-    def get(self, poll: str, userId: int, dateId: int): return GetSearchAnswer(poll, userId, dateId).run()
+    def get(self, poll: str, userId: int, dateId: int) -> str: return GetSearchAnswer(poll, userId, dateId).run().toJSON()
 
 
 class SessionEndpoint(Resource):
-    def get(self, poll: str, id: str): return GetSession(poll, id).run()
+    def get(self, poll: str, id: str) -> str: return GetSession(poll, id).run().toJSON()
     
     @history
-    def post(self, poll: str, id: str): return CreateSession(poll, id, body(flask.request, 'user_id')).run()
+    def post(self, poll: str, id: str) -> str: return CreateSession(poll, id, body(flask.request, 'user_id')).run().toJSON()
 
 
 
 
 api.add_resource(PollEndpoint, '/<string:poll>')
 api.add_resource(InstrumentsEndpoint, '/<string:poll>/instrument')
 api.add_resource(UsersEndpoint, '/<string:poll>/user')
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.57/popoll_backend/model/db/user_instruments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from typing import Any, List
+from __future__ import annotations
+
+import sqlite3
+
+from typing import Any, List, Optional, Tuple
 
 from popoll_backend.model import Payload
 
-class Answer(Payload):
+
+class UserInstruments(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.user_id: int = data[1]
-        self.date_id: int = data[2]
-        self.response: bool = bool(data[3])
+        self.instrument_id: int = data[2]
+        self.is_main: bool = bool(data[3])
 
     @classmethod
     def create_table(cls):
-        return """ CREATE TABLE IF NOT EXISTS answers (
-            id integer PRIMARY KEY AUTOINCREMENT,
+        return """ CREATE TABLE IF NOT EXISTS user_instruments (
+            id integer PRIMARY KEY,
             user_id integer NOT NULL REFERENCES users(id) ON DELETE CASCADE,
-            date_id integer NOT NULL REFERENCES dates(id) ON DELETE CASCADE,
-            response boolean NOT NULL,
-            UNIQUE(user_id, date_id)
-        ); """
+            instrument_id integer NOT NULL REFERENCES instruments(id) ON DELETE CASCADE,
+            is_main boolean NOT NULL
+        ); """
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/db/date.py` & `popoll_backend-0.0.57/popoll_backend/model/db/date.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from __future__ import annotations
 import datetime
+import sqlite3
 from typing import Any, List, Optional
 
 from popoll_backend.model import Payload
+from popoll_backend.model.db import fetchall, fetchone
 
 
 class Date(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.title: str = data[1]
@@ -17,8 +20,8 @@
     def create_table(cls):
         return """ CREATE TABLE IF NOT EXISTS dates (
             id integer PRIMARY KEY AUTOINCREMENT,
             title text NOT NULL,
             date text NOT NULL,
             time text,
             end_time text
-        ); """
+        ); """
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/db/session.py` & `popoll_backend-0.0.57/popoll_backend/model/db/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+from __future__ import annotations
+
+import datetime
+import sqlite3
 from typing import Any, List
 
 from popoll_backend.model import Payload
+from popoll_backend.model.db import fetchone
 
 
 class Session(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.session_id: str = data[1]
@@ -13,8 +18,8 @@
     @classmethod
     def create_table(cls):
         return """CREATE TABLE IF NOT EXISTS sessions (
             id integer PRIMARY KEY,
             session_id text NOT NULL,
             user_id integer NOT NULL REFERENCES users(id) ON DELETE CASCADE,
             datetime text NOT NULL
-        );"""
+        );"""
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.57/popoll_backend/model/db/answer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import sqlite3
+
 from typing import Any, List
 
 from popoll_backend.model import Payload
+from popoll_backend.model.db import fetchall, fetchone
 
-
-class UserInstruments(Payload):
+class Answer(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.user_id: int = data[1]
-        self.instrument_id: int = data[2]
-        self.is_main: bool = bool(data[3])
+        self.date_id: int = data[2]
+        self.response: bool = bool(data[3])
 
     @classmethod
     def create_table(cls):
-        return """ CREATE TABLE IF NOT EXISTS user_instruments (
-            id integer PRIMARY KEY,
+        return """ CREATE TABLE IF NOT EXISTS answers (
+            id integer PRIMARY KEY AUTOINCREMENT,
             user_id integer NOT NULL REFERENCES users(id) ON DELETE CASCADE,
-            instrument_id integer,
-            is_main boolean NOT NULL
-        ); """
+            date_id integer NOT NULL REFERENCES dates(id) ON DELETE CASCADE,
+            response boolean NOT NULL,
+            UNIQUE(user_id, date_id)
+        ); """
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/payload/date_payload.py` & `popoll_backend-0.0.57/popoll_backend/model/payload/date_details.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model import Payload
 
 def getUser(users: List[User], id: int) -> User:
     return [user for user in users if user.id == id][0]
 
 def getInstrument(instruments: List[Instrument], id: int) -> Instrument:
-    return [instrument for instrument in instruments if instrument.instrument.id == id][0]
+    return [instrument for instrument in instruments if instrument.id == id][0]
 
 def getMainInstrument(instruments: List[Instrument], user_instruments: List[UserInstruments], user: User) -> Instrument:
     return getInstrument(instruments, [user_instrument.instrument_id for user_instrument in user_instruments if user_instrument.user_id == user.id and user_instrument.is_main][0])
 
 def getSecondInstruments(instruments: List[Instrument], user_instruments: List[UserInstruments], user: User) -> List[Instrument]:
     return [getInstrument(instruments, iid) for iid in [user_instrument.instrument_id for user_instrument in user_instruments if user_instrument.user_id == user.id and not user_instrument.is_main]]
 
@@ -22,29 +22,23 @@
     res: List[Answer] = [answer for answer in answers if answer.user_id == user_id]
     if len(res) == 0:
         return None
     if len(res) > 1:
         print('WEIRD CASE')
     return res[0]
 
-class _DateInstrumentAnswerPayload:
-    
-    def __init__(self, instrument: Instrument):
-        self.instrument = instrument
-        self.is_used_this_date = False
-        self.is_used_antoher_date = False
 class _DateAnswerPayload:
     
     def __init__(self, answer: Answer, user: User, instrument: Instrument, is_main_instrument: bool):
         self.answer = answer
         self.user = user
         self.instrument = instrument
         self.is_main_instrument = is_main_instrument
 
-class DatePayload(Payload):
+class DateDetails(Payload):
     
     def __init__(self, date: Date, answers: List[Answer], users: List[User], instruments: List[Instrument], user_instruments: List[UserInstruments]):
         self.date: Date = date
         self.answers: List[_DateAnswerPayload] = []
         for user in users:
             answer = getAnswer(answers, user.id)
             self.answers.append(_DateAnswerPayload(answer, user, getMainInstrument(instruments, user_instruments, user), True))
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.57/popoll_backend/model/payload/history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import contextlib
 import datetime
 import flask
 import json
-import jsonpickle
 
 from popoll_backend.model import Payload
 
 class History(Payload):
     
     def __init__(self, request: flask.Request, response, kwargs):
         self.date = datetime.datetime.now().isoformat(sep='T', timespec='auto')
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/payload/user.py` & `popoll_backend-0.0.57/popoll_backend/model/payload/user_with_instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, List
 from popoll_backend.model import Payload
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user_instruments import UserInstruments
 
 
-class UserOut(Payload):
+class UserWithInstruments(Payload):
     
-    def __init__(self, user: User, instruments: Instrument, user_instruments: List[UserInstruments]):
+    def __init__(self, user: User, instruments: List[Instrument], user_instruments: List[UserInstruments]):
         self.user = user
         self.main_instrument: Instrument = self.getInstrument(instruments, self.getInstrumentIds(user_instruments, user.id, True)[0])
         self.instruments: List[Instrument] = self.getInstruments(instruments, self.getInstrumentIds(user_instruments, user.id, False))
         
     def getInstrumentIds(self, user_instruments: List[UserInstruments], user_id: int, is_main: bool):
         return [user_instrument.instrument_id for user_instrument in user_instruments if user_instrument.user_id == user_id and user_instrument.is_main == is_main]
     
     def getInstruments(self, instruments: List[Instrument], ids: List[int]):
-        return [instrument for instrument in instruments if instrument.instrument.id in ids]
+        return [instrument for instrument in instruments if instrument.id in ids]
     
     def getInstrument(self, instruments: List[Instrument], id: int):
-        return [instrument for instrument in instruments if instrument.instrument.id == id][0]
+        return [instrument for instrument in instruments if instrument.id == id][0]
```

### Comparing `popoll_backend-0.0.56/popoll_backend/model/payload/user_payload.py` & `popoll_backend-0.0.57/popoll_backend/model/payload/user_details.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from typing import List, Optional
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
-from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.model.db.user import User
-from popoll_backend.model.db.user_instruments import UserInstruments
 from popoll_backend.model import Payload
-from popoll_backend.model.payload.user import UserOut
+from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 
-class _UserDateOutput():
+class UserDetailsDate():
     
-    def __init__(self, user: UserOut, date: Date, answers: List[Answer]):
+    def __init__(self, user: UserWithInstruments, date: Date, answers: List[Answer]):
         self.date: Date = date
-        _ans = [a for a in answers if a.user_id == user.user.id and a.date_id == date.id]
+        _ans = [a for a in answers if a.user_id == user.id and a.date_id == date.id]
         self.answer: Optional[Answer] = _ans[0] if len(_ans) > 0 else None
         
 
-class UserPayload(Payload):
+class UserDetails(Payload):
     
-    def __init__(self, user: UserOut, answers: List[Answer], dates: List[Date]):
-        self.user: UserOut = user
-        self.dates: List[_UserDateOutput] = [_UserDateOutput(user, date, answers) for date in dates]
+    def __init__(self, user: UserWithInstruments, answers: List[Answer], dates: List[Date]):
+        self.user: UserWithInstruments = user
+        self.dates: List[UserDetailsDate] = [UserDetailsDate(user, date, answers) for date in dates]
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.57/popoll_backend/query/create_session.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,25 @@
+import datetime
 import sqlite3
 
-import flask
-
-from popoll_backend.model import Payload
+from popoll_backend.model.db.session import Session
 from popoll_backend.query import Query
-from popoll_backend.query.get_answer import GetAnswer
 
 
-class CreateAnswer(Query):
-    
-    user_id: int
-    date_id: int
+class CreateSession(Query):
     
     id: int
     
-    def __init__(self, poll:str, user_id: int, date_id: int):
+    def __init__(self, poll: str, id: str, user_id: int):
         super().__init__(poll)
+        self.id = id
         self.user_id = user_id
-        self.date_id = date_id
-    
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO answers(user_id, date_id, response) VALUES (?, ?, ?)', (self.user_id, self.date_id, True))
-        self.id = cursor.lastrowid
-        
-    
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetAnswer(self.poll, self.id).run(cursor)
+
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('DELETE FROM sessions WHERE session_id=?', (self.id,))
+        return cursor.execute('INSERT INTO sessions(session_id, user_id, datetime) VALUES(?, ?, ?)', (self.id, self.user_id, self.getNow())).lastrowid
+
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Session:
+        return self.fetchlast(cursor.execute('SELECT * FROM sessions WHERE session_id=?', (self.id,)), Session)
     
-    def error(self, e: sqlite3.Error):
-        if isinstance(e, sqlite3.IntegrityError):
-            if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
-                flask.abort(400, f'Answer for this user already exists. PUT should be triggered instead.')
+    def getNow(self) -> str:
+        return datetime.datetime.now().isoformat(sep='T', timespec='auto')
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/create_date.py` & `popoll_backend-0.0.57/popoll_backend/query/update_date.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import datetime
 import sqlite3
 from typing import Optional
 
-from popoll_backend.model import Payload
+from popoll_backend.model.db.date import Date
 from popoll_backend.query import Query
-from popoll_backend.query.get_date import GetDate
 
 
-class CreateDate(Query):
+class UpdateDate(Query):
     
+    id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
     
-    id: int
-    
-    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
+    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
         super().__init__(poll)
+        self.id = id
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
-    
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO dates(title, date, time, end_time) VALUES (?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time))
-        self.id = cursor.lastrowid
         
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetDate(self.poll, self.id, False).run(cursor)
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.id))
+    
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
+        return self.fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.57/popoll_backend/query/create_instrument.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import sqlite3
 
-from popoll_backend.model import Payload
+from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.query import Query
-from popoll_backend.query.get_instrument import GetInstrument
 
 
 class CreateInstrument(Query):
     
-    instrument_id: int
     name: str
     rank: int
     
+    instrument_id: int
+    
     def __init__(self, poll: str, name: str, rank: int):
         super().__init__(poll)
         self.name = name
         self.rank = rank
-        
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO instruments.instruments(name, rank) VALUES (?, ?)', (self.name, self.rank))
-        self.instrument_id = cursor.lastrowid
-        
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetInstrument(self.poll, self.instrument_id).run(cursor)
+       
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        self.instrument_id = cursor.execute('INSERT INTO instruments.instruments(name, rank) VALUES (?,?)', (self.name, self.rank)).lastrowid
+    
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Instrument:
+        return self.fetchlast(cursor.execute('SELECT * FROM instruments.instruments WHERE id=?', (self.id,)), Instrument)
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.57/popoll_backend/query/get_date_details.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 import sqlite3
-from typing import List
 
-import flask
-
-from popoll_backend.model import Payload
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.model.db.date import Date
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.model.db.option import Option
-from popoll_backend.model.db.session import Session
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
-from popoll_backend.model.payload.id_payload import IdPayload
+from popoll_backend.model.payload.date_details import DateDetails
 from popoll_backend.query import Query
 
 
-class CreatePoll(Query):
-    
-    fail_if_db_exists: bool = True
-    fail_if_db_not_exists: bool = False
+class GetDateDetails(Query):
     
-    name: str
-    instruments: List[str]
-    color: str
+    id: int
     
-    def __init__(self, poll:str, name: str, instruments: List[str], color: str):
+    def __init__(self, poll: str, id: int):
         super().__init__(poll)
-        self.name = name
-        self.instruments = instruments
-        self.color = color
-    
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute(Option.create_table())
-        cursor.execute('INSERT INTO options(name, color) values(?, ?)', (self.name, self.color))
-        cursor.execute(Date.create_table())
-        cursor.execute(User.create_table())
-        cursor.execute(Answer.create_table())
-        cursor.execute(UserInstruments.create_table())
-        cursor.execute(Session.create_table())
-    
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return IdPayload(0)
+        self.id = id
+
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        pass
+
+    def buildResponse(self, cursor: sqlite3.Cursor) -> DateDetails:
+        globally_used_instruments = [row[0] for row in cursor.execute('SELECT DISTINCT instrument_id FROM user_instruments').fetchall()]
+        return DateDetails(
+            date=self.fetchlast(cursor.execute('SELECT * FROM dates where id=?', (self.id,)), Date), 
+            answers=self.fetchall(cursor.execute('SELECT * FROM answers where date_id=?', (self.id,)), Answer),
+            users=self.fetchall(cursor.execute('SELECT * FROM users ORDER BY name COLLATE NOCASE'), User),     
+            instruments=[instr for instr in self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments],
+            user_instruments=self.fetchall(cursor.execute('SELECT * FROM user_instruments'), UserInstruments)
+        )
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/create_user.py` & `popoll_backend-0.0.57/popoll_backend/query/create_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import flask
 import sqlite3
 from typing import List
 
 from popoll_backend.model import Payload
+from popoll_backend.model.db.instrument import Instrument
+from popoll_backend.model.db.user import User
+from popoll_backend.model.db.user_instruments import UserInstruments
+from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.query import Query
-from popoll_backend.query.get_user import GetUser
 
 
 class CreateUser(Query):
     
     name: str
     main_instrument: int
     instruments: List[int]
@@ -17,20 +20,23 @@
     
     def __init__(self, poll: str, name: str, main_instrument: int, instruments: List[int]):
         super().__init__(poll)
         self.name = name
         self.main_instrument = main_instrument
         self.instruments = instruments
     
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO users(name) VALUES (?)', (self.name,))
-        self.id = cursor.lastrowid
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        self.id = cursor.execute('INSERT INTO users(name) VALUES(?)', (self.name,)).lastrowid
         rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
         cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetUser(self.poll, self.id, details=False).run(cursor)
+        return UserWithInstruments(
+            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
+            user_instruments=self.fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
+        )
     
     def error(self, e: sqlite3.Error):
         if isinstance(e, sqlite3.IntegrityError):
             if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
-                flask.abort(400, f'User with name {self.name} already exists.')
+                flask.abort(409, f'User with name {self.name} already exists.')
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.57/popoll_backend/query/delete_instrument.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import sqlite3
 from popoll_backend.model import Payload
+from popoll_backend.model.db.instrument import Instrument
+from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
 
 
-class DeleteAnswer(Query):
+class DeleteInstrument(Query):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('DELETE FROM answers WHERE id=?', (self.id,))
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('DELETE FROM instruments.instruments WHERE id=?', (self.id,))
     
-    def buildResponse(self, _: sqlite3.Cursor) -> Payload:
-        return IdPayload(self.id)
+    def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
+        return Empty()
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.57/popoll_backend/query/delete_date.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
+from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
 
 
 class DeleteDate(Query):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
-    def process(self, cursor: sqlite3.Cursor):
+    def process(self, cursor: sqlite3.Cursor) -> None:
         cursor.execute('DELETE FROM dates WHERE id=?', (self.id,))
     
-    def buildResponse(self, _: sqlite3.Cursor) -> Payload:
-        return IdPayload(self.id)
+    def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
+        return Empty()
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/delete_instrument.py` & `popoll_backend-0.0.57/popoll_backend/query/delete_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
+from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
 
 
-class DeleteInstrument(Query):
+class DeleteUser(Query):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('DELETE FROM instruments.instruments WHERE id=?', (self.id,))
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
     
-    def buildResponse(self, _: sqlite3.Cursor) -> Payload:
-        return IdPayload(self.id)
+    def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
+        return Empty()
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.57/popoll_backend/query/delete_answer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sqlite3
 from popoll_backend.model import Payload
+from popoll_backend.model.payload.empty import Empty
 from popoll_backend.model.payload.id_payload import IdPayload
 from popoll_backend.query import Query
 
 
-class DeleteUser(Query):
+class DeleteAnswer(Query):
     
     id: int
     
     def __init__(self, poll: str, id: int):
         super().__init__(poll)
         self.id = id
     
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('DELETE FROM users WHERE id=?', (self.id,))
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        cursor.execute('DELETE FROM answers WHERE id=?', (self.id,))
     
-    def buildResponse(self, _: sqlite3.Cursor) -> Payload:
-        return IdPayload(self.id)
+    def buildResponse(self, _: sqlite3.Cursor) -> IdPayload:
+        return Empty()
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/get_answer.py` & `popoll_backend-0.0.57/popoll_backend/query/update_answer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import sqlite3
-from typing import List
+from typing import Optional
 
 from popoll_backend.model import Payload
 from popoll_backend.model.db.answer import Answer
 from popoll_backend.query import Query
+from popoll_backend.query.get_answer import GetAnswer
 
 
-class GetAnswer(Query):
+class UpdateAnswer(Query):
     
     id: int
+    response: Optional[bool]
     
-    def __init__(self, poll: str, id: int):
+    def __init__(self, poll:str, id: int, response: Optional[bool]):
         super().__init__(poll)
         self.id = id
-
+        self.response = response
+    
     def process(self, cursor: sqlite3.Cursor):
-        pass
+        cursor.execute('UPDATE answers SET response=? WHERE id=?', (self.response, self.id))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return self.selectItem(cursor, 'SELECT * from answers where id=?', self.id, Answer)
+        return self.fetchlast(cursor.execute('SELECT * FROM answers WHERE id=?', (self.id,)), Answer)
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.57/popoll_backend/query/get_users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import sqlite3
 from typing import List
 
-from popoll_backend.model import Payload
-from popoll_backend.model.db.date import Date
-from popoll_backend.model.payload.dates_payload import DatesPayload
+from popoll_backend.model.db.instrument import Instrument
+from popoll_backend.model.db.user import User
+from popoll_backend.model.db.user_instruments import UserInstruments
+from popoll_backend.model.payload.users import Users
 from popoll_backend.query import Query
 
 
-class GetDates(Query):
-    
-    dates: List[Date]
+class GetUsers(Query):
     
     def __init__(self, poll: str):
         super().__init__(poll)
+    
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        pass
 
-    def process(self, cursor: sqlite3.Cursor):
-        self.dates = [Date(row) for row in cursor.execute('SELECT * FROM dates ORDER BY date, time').fetchall()]
-        
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return DatesPayload(self.dates)
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Users:
+        return Users(self.fetchall(cursor.execute('SELECT * FROM users ORDER BY name COLLATE NOCASE'), User))
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/get_instrument.py` & `popoll_backend-0.0.57/popoll_backend/query/get_instruments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sqlite3
+from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.model.payload.instrument_payload import InstrumentPayload
+from popoll_backend.model.payload.instruments import Instruments
 from popoll_backend.query import Query
 
 
-class GetInstrument(Query):
+class GetInstruments(Query):
     
-    id: int
+    instruments: List[Instrument]
     
-    def __init__(self, poll: str, id: int):
+    def __init__(self, poll: str):
         super().__init__(poll)
-        self.id = id
-    
-    def process(self, cursor: sqlite3.Cursor):
+
+    def process(self, cursor: sqlite3.Cursor) -> None:
         pass
-        
-    def buildResponse(self, cursor: sqlite3.Cursor) -> InstrumentPayload:
-        instrument: Instrument = self.selectItem(cursor, 'SELECT * FROM instruments.instruments WHERE id=?', self.id, Instrument)
-        all_used_instruments = cursor.execute('SELECT COUNT(instrument_id) FROM user_instruments WHERE instrument_id = ?', (self.id,)).fetchall()
-        return InstrumentPayload(instrument, all_used_instruments[0][0] > 0)
+            
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Instruments:
+        globally_used_instruments = [row[0] for row in cursor.execute('SELECT DISTINCT instrument_id FROM user_instruments').fetchall()]
+        return Instruments([instr for instr in self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument) if instr.id in globally_used_instruments])
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.57/popoll_backend/query/get_user_with_instruments.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import sqlite3
-from typing import List
 
 from popoll_backend.model.db.instrument import Instrument
-from popoll_backend.model.payload.instruments_payload import InstrumentsPayload
+from popoll_backend.model.db.user import User
+from popoll_backend.model.db.user_instruments import UserInstruments
+from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.query import Query
 
 
-class GetInstruments(Query):
+class GetUserWithInstruments(Query):
     
-    instruments: List[Instrument]
-    all_used_instruments: List[int]
+    id: int
     
-    def __init__(self, poll: str):
+    def __init__(self, poll: str, id: int):
         super().__init__(poll)
+        self.id = id
     
-    def process(self, cursor: sqlite3.Cursor):
-        self.instruments = [Instrument(row) for row in cursor.execute('SELECT * from instruments.instruments ORDER BY rank').fetchall()]
-        self.all_used_instruments = [i[0] for i in cursor.execute('SELECT DISTINCT instrument_id FROM user_instruments').fetchall()]
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        pass
         
-    def buildResponse(self, cursor: sqlite3.Cursor) -> InstrumentsPayload:
-        return InstrumentsPayload(self.instruments, self.all_used_instruments)
+    def buildResponse(self, cursor: sqlite3.Cursor) -> UserWithInstruments:
+        return UserWithInstruments(
+            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments ORDER BY rank'), Instrument),
+            user_instruments=self.fetchall(cursor.execute('SELECT * FROM user_instruments WHERE user_id=?', (self.id,)), UserInstruments)
+        )
+        
+        
+
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/get_users.py` & `popoll_backend-0.0.57/popoll_backend/query/update_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 import sqlite3
 from typing import List
 
+import flask
+
 from popoll_backend.model import Payload
 from popoll_backend.model.db.instrument import Instrument
 from popoll_backend.model.db.user import User
 from popoll_backend.model.db.user_instruments import UserInstruments
-from popoll_backend.model.payload.user import UserOut
-from popoll_backend.model.payload.users_payload import UsersPayload
-from popoll_backend.model.payload.users_payload_details import UsersPayloadDetails
+from popoll_backend.model.payload.user_with_instruments import UserWithInstruments
 from popoll_backend.query import Query
-from popoll_backend.query.get_instruments import GetInstruments
 
 
-class GetUsers(Query):
-    
-    details: bool
+class UpdateUser(Query):
     
-    users: List[User]
-    instruments: List[Instrument]
-    user_instruments: List[UserInstruments]
+    id: int
+    name: str
+    main_instrument: int
+    instruments: List[int]
     
-    def __init__(self, poll: str, details: bool = False):
+    def __init__(self, poll, id, name, main_instrument, instruments):
         super().__init__(poll)
-        self.details = details
+        self.id = id
+        self.name = name
+        self.main_instrument = main_instrument
+        self.instruments = instruments
     
     def process(self, cursor: sqlite3.Cursor):
-        self.users = [User(data) for data in cursor.execute('SELECT * from users ORDER BY name COLLATE NOCASE').fetchall()]       
-        if self.details:
-            self.instruments: List[Instrument] = GetInstruments(self.poll).run(cursor).instruments
-            self.user_instruments: List[UserInstruments] = [UserInstruments(data) for data in cursor.execute('SELECT * from user_instruments').fetchall()]
-
+        cursor.execute('UPDATE users SET name=? WHERE id=?', (self.name, self.id))
+        cursor.execute('DELETE FROM user_instruments WHERE user_id=?', (self.id,))
+        rows = [(self.id, self.main_instrument, True)] + [(self.id, instru, False) for instru in self.instruments if not instru == self.main_instrument]
+        cursor.executemany('INSERT INTO user_instruments(user_id, instrument_id, is_main) VALUES(?, ?, ?)', rows)
+    
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        if not self.details:
-            return UsersPayload(self.users)
-        users_out = [UserOut(_user, self.instruments, self.user_instruments) for _user in self.users]    
-        return UsersPayloadDetails(users_out)
+        return UserWithInstruments(
+            user=self.fetchlast(cursor.execute('SELECT * FROM users WHERE id=?', (self.id,)), User), 
+            instruments=self.fetchall(cursor.execute('SELECT * FROM instruments'), Instrument), 
+            user_instruments=self.fetchall(cursor.execute('SELECT * from user_instruments where user_id=?', (self.id,)), UserInstruments)
+        )
+    
+    def error(self, e: sqlite3.Error):
+        if isinstance(e, sqlite3.IntegrityError):
+            if e.sqlite_errorcode == sqlite3.SQLITE_CONSTRAINT_UNIQUE:
+                flask.abort(409, f'User with name {self.name} already exists, cannot update.')
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.57/popoll_backend/query/get_dates.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import sqlite3
-from typing import Optional
+from typing import List
 
-from popoll_backend.model import Payload
-from popoll_backend.model.db.answer import Answer
+from popoll_backend.model.db.date import Date
+from popoll_backend.model.payload.dates import Dates
 from popoll_backend.query import Query
-from popoll_backend.query.get_answer import GetAnswer
 
 
-class UpdateAnswer(Query):
+class GetDates(Query):
     
-    id: int
-    response: Optional[bool]
+    dates: List[Date]
     
-    def __init__(self, poll:str, id: int, response: Optional[bool]):
+    def __init__(self, poll: str):
         super().__init__(poll)
-        self.id = id
-        self.response = response
-    
+
     def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('UPDATE answers SET response=? WHERE id=?', (self.response, self.id))
-    
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetAnswer(self.poll, self.id).run(cursor)
+        pass
+        
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Dates:
+        return Dates(self.fetchall(cursor.execute('SELECT * FROM dates ORDER BY date, time'), Date))
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/update_date.py` & `popoll_backend-0.0.57/popoll_backend/query/create_date.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import datetime
 import sqlite3
 from typing import Optional
 
-from popoll_backend.model import Payload
+from popoll_backend.model.db.date import Date
 from popoll_backend.query import Query
-from popoll_backend.query.get_date import GetDate
 
 
-class UpdateDate(Query):
+class CreateDate(Query):
     
-    id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
     end_time: Optional[datetime.time]
     
-    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
+    id: int
+    
+    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
         super().__init__(poll)
-        self.id = id
         self.title = title
         self.date = date
         self.time = time
         self.end_time = end_time
-        
-    def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.id))
     
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetDate(self.poll, self.id, False).run(cursor)
+    def process(self, cursor: sqlite3.Cursor) -> None:
+        self.id = cursor.execute('INSERT INTO dates(title, date, time, end_time) VALUES (?, ?, ?, ?)', (self.title, self.date, self.time, self.end_time)).lastrowid
+        
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Date:
+        return self.fetchlast(cursor.execute('SELECT * FROM dates WHERE id=?', (self.id,)), Date)
```

### Comparing `popoll_backend-0.0.56/popoll_backend/query/update_poll.py` & `popoll_backend-0.0.57/popoll_backend/query/update_poll.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sqlite3
 
-from popoll_backend.model import Payload
+from popoll_backend.model.db.option import Option
 from popoll_backend.query import Query
-from popoll_backend.query.get_poll import GetPoll
 
 
 class UpdatePoll(Query):
     
     name: str
     color: str
     
     def __init__(self, poll: str, name: str, color: str):
         super().__init__(poll)
         self.name = name
         self.color = color
         
-    def process(self, cursor: sqlite3.Cursor):
+    def process(self, cursor: sqlite3.Cursor) -> None:
         cursor.execute('UPDATE options SET name=?, color=?', (self.name, self.color))
     
-    def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetPoll(self.poll).run(cursor)
+    def buildResponse(self, cursor: sqlite3.Cursor) -> Option:
+        return Option(cursor.execute('SELECT * FROM options').fetchone())
```

### Comparing `popoll_backend-0.0.56/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.57/popoll_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.56
+Version: 0.0.57
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.56/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.57/popoll_backend.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,64 +12,65 @@
 popoll_backend/model/db/date.py
 popoll_backend/model/db/instrument.py
 popoll_backend/model/db/option.py
 popoll_backend/model/db/session.py
 popoll_backend/model/db/user.py
 popoll_backend/model/db/user_instruments.py
 popoll_backend/model/payload/__init__.py
-popoll_backend/model/payload/date_payload.py
-popoll_backend/model/payload/dates_payload.py
+popoll_backend/model/payload/date_details.py
+popoll_backend/model/payload/dates.py
+popoll_backend/model/payload/empty.py
 popoll_backend/model/payload/history.py
 popoll_backend/model/payload/id_payload.py
-popoll_backend/model/payload/instrument_payload.py
-popoll_backend/model/payload/instruments_payload.py
-popoll_backend/model/payload/user.py
-popoll_backend/model/payload/user_payload.py
-popoll_backend/model/payload/users_payload.py
+popoll_backend/model/payload/instruments.py
+popoll_backend/model/payload/user_details.py
+popoll_backend/model/payload/user_with_instruments.py
+popoll_backend/model/payload/users.py
 popoll_backend/model/payload/users_payload_details.py
 popoll_backend/query/__init__.py
 popoll_backend/query/create_answer.py
 popoll_backend/query/create_date.py
 popoll_backend/query/create_instrument.py
 popoll_backend/query/create_poll.py
 popoll_backend/query/create_session.py
 popoll_backend/query/create_user.py
 popoll_backend/query/delete_answer.py
 popoll_backend/query/delete_date.py
 popoll_backend/query/delete_instrument.py
 popoll_backend/query/delete_user.py
+popoll_backend/query/get_all_instruments.py
 popoll_backend/query/get_answer.py
 popoll_backend/query/get_date.py
+popoll_backend/query/get_date_details.py
 popoll_backend/query/get_dates.py
 popoll_backend/query/get_instrument.py
 popoll_backend/query/get_instruments.py
 popoll_backend/query/get_poll.py
 popoll_backend/query/get_search_answer.py
 popoll_backend/query/get_session.py
-popoll_backend/query/get_user.py
+popoll_backend/query/get_user_details.py
+popoll_backend/query/get_user_with_instruments.py
 popoll_backend/query/get_users.py
 popoll_backend/query/update_answer.py
 popoll_backend/query/update_date.py
 popoll_backend/query/update_poll.py
 popoll_backend/query/update_user.py
-tests/test_01_db_creation.py
-tests/test_02_simple_adds.py
-tests/test_03_no_duplicates.py
-tests/test_04_update_user_entry.py
-tests/test_05_update_date_entry.py
-tests/test_06_update_answer_entry.py
-tests/test_07_delete_user_entry.py
-tests/test_08_delete_date_entry.py
-tests/test_09_delete_user_date_entries.py
-tests/test_10_get_users.py
-tests/test_11_get_users_sort_name.py
-tests/test_12_get_dates_sort_dateTime.py
-tests/test_13_history.py
-tests/test_14_get_answers_user.py
-tests/test_15_multi_instruments.py
-tests/test_16_get_date.py
-tests/test_17_get_instruments.py
-tests/test_19_delete_database.py
-tests/test_20_add_answer_no_dupe.py
-tests/test_21_get_dates.py
-tests/test_22_add_instrument.py
-tests/test_23_get_instruments_with_is_used.py
+tests/test_01_get_poll.py
+tests/test_02_create_poll.py
+tests/test_03_update_poll.py
+tests/test_04_get_instruments.py
+tests/test_08_get_users.py
+tests/test_09_create_user.py
+tests/test_10_get_user.py
+tests/test_11_update_user.py
+tests/test_12_delete_user.py
+tests/test_13_get_dates.py
+tests/test_14_create_date.py
+tests/test_15_get_date.py
+tests/test_16_update_date.py
+tests/test_17_delete_date.py
+tests/test_18_create_answer.py
+tests/test_19_update_answer.py
+tests/test_20_delete_answer.py
+tests/test_21_get_answer.py
+tests/test_22_get_search_answer.py
+tests/test_23_get_create_session.py
```

### Comparing `popoll_backend-0.0.56/pyproject.toml` & `popoll_backend-0.0.57/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.56"
+version = "0.0.57"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.56/tests/test_01_db_creation.py` & `popoll_backend-0.0.57/tests/test_01_get_poll.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from tests import IntegrationTest
 
-class TestDBCreation(IntegrationTest):
+class TestGetPoll(IntegrationTest):
 
     def test_db_creation(self):
-        _json = self.get_instruments()
-        
-        assert _json['instruments'][0]['instrument']['id'] == self.instru1_id
-        assert _json['instruments'][0]['instrument']['name'] == self.INSTRU1
-        assert _json['instruments'][1]['instrument']['id'] == self.instru3_id
-        assert _json['instruments'][1]['instrument']['name'] == self.INSTRU3
-        assert _json['instruments'][2]['instrument']['id'] == self.instru2_id
-        assert _json['instruments'][2]['instrument']['name'] == self.INSTRU2
+        _json = self.get_instruments(False)
+        self.assertEqual(9, len(_json['instruments']))
+        self.assertEqual(self.instru1_id, _json['instruments'][0]['id'])
+        self.assertEqual(self.INSTRU1, _json['instruments'][0]['name'])
+        self.assertEqual(self.instru2_id, _json['instruments'][1]['id'])
+        self.assertEqual(self.INSTRU2, _json['instruments'][1]['name'])
+        self.assertEqual(self.instru3_id, _json['instruments'][2]['id'])
+        self.assertEqual(self.INSTRU3, _json['instruments'][2]['name'])
+
+    def test_get_poll(self):
+        _json = self.get_poll()
+        self.assertEqual('TESTTEST', _json['name'])
+        self.assertEqual('#ff8b00', _json['color'])
```

### Comparing `popoll_backend-0.0.56/tests/test_07_delete_user_entry.py` & `popoll_backend-0.0.57/tests/test_12_delete_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from tests import IntegrationTest
 
-class TestDeleteUserEntry(IntegrationTest):
+class TestDeleteUser(IntegrationTest):
 
     def setUp(self):
         super().setUp()
-        self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.user2_id = self.create_user('user2', self.instru2_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
-        self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
+        self.user1_id = self.create_user('user1', self.instru1_id, [])['user']['id']
+        self.user2_id = self.create_user('user2', self.instru1_id, [])['user']['id']
         
-    def test_delete_user_entry(self):
-        deleted_user_id = self.delete_user(self.user1_id)
-        assert deleted_user_id == self.user1_id
-        _json = self.get_users()
-        assert len(_json['users']) == 1
-        assert _json['users'][0]['user']['name'] == 'user2'        
+    def test_delete_user(self):
+        _json = self.delete_user(self.user1_id)
+        self.assertEqual({}, _json)
+
+    def test_delete_user_invalid(self):
+        _rs = self.delete_user(99, fail=True)
+        self.assertEqual(200, _rs.status_code)
+        self.assertEqual({}, _rs.json)
```

### Comparing `popoll_backend-0.0.56/tests/test_20_add_answer_no_dupe.py` & `popoll_backend-0.0.57/tests/test_21_get_answer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from tests import IntegrationTest
 
-class TestAddAnswerNoDupe(IntegrationTest):
+class TestGetAnswer(IntegrationTest):
 
     def setUp(self):
         super().setUp()
-        self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
-        self.answer1_id = self.create_answer(self.user1_id, self.date1_id)
-
-
-    def test_delete_database(self):            
-        rs = self.create_answer(self.user1_id, self.date1_id, fail=True)
-        assert rs.status_code == 400
+        self.user1_id = self.create_user('user1', self.instru2_id, [self.instru1_id])['user']['id']
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
+        self.answer1_id = self.create_answer(self.user1_id, self.date1_id)['id']
         
-
+    def test_get_answer_answerId(self):
+        _json = self.get_answer(self.answer1_id)
+        self.assertAnswer(_json, self.answer1_id, self.user1_id, self.date1_id, True)
```

### Comparing `popoll_backend-0.0.56/tests/test_21_get_dates.py` & `popoll_backend-0.0.57/tests/test_10_get_user.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from tests import IntegrationTest
 
-class TestAddAnswerNoDupe(IntegrationTest):
+class TestGetUser(IntegrationTest):
 
     def setUp(self):
         super().setUp()
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
-        self.date2_id = self.create_date(date='2025-03-11', time=None, title='secondDate', end_time=None)
-
-    def _assert_date(self, e_id, e_date, e_time, e_title, actual):
-        assert e_id == actual['id']
-        assert e_title == actual['title']
-        assert e_date == actual['date']
-        assert e_time == actual['time']
-
-    def test_get_dates(self):
-        rs = self.get_dates()
-        assert len(rs['dates']) == 2
-        self._assert_date(self.date1_id, '2025-03-10', '15:00:00', 'firstDate', rs['dates'][0])
-        self._assert_date(self.date2_id, '2025-03-11', None, 'secondDate', rs['dates'][1])
+        self.user1_id = self.create_user('user1', self.instru2_id, [self.instru3_id, self.instru1_id])['user']['id']
         
+    def test_get_user(self):
+        _json = self.get_user(self.user1_id, False)
+        self.assertUserWithInstruments(_json, self.user1_id, 'user1', self.instru2_id, [self.instru1_id, self.instru3_id])
 
+    def test_get_user_details(self):
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')['id']
+        self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)['id']
+        _json = self.get_user(self.user1_id, True)
+        self.assertUser(_json['user'], self.user1_id, 'user1')
+        self.assertEqual(1, len(_json['dates']))
+        self.assertDate(_json['dates'][0]['date'], self.date1_id, '2025-03-10', '15:00:00', '18:00:00', 'firstDate')
+        self.assertAnswer(_json['dates'][0]['answer'], self.answer1_id, self.user1_id, self.date1_id, True)
```

