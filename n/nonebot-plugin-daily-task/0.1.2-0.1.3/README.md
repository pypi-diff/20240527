# Comparing `tmp/nonebot_plugin_daily_task-0.1.2.tar.gz` & `tmp/nonebot_plugin_daily_task-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_daily_task-0.1.2.tar", last modified: Sun May 26 16:34:03 2024, max compression
+gzip compressed data, was "nonebot_plugin_daily_task-0.1.3.tar", last modified: Mon May 27 12:05:20 2024, max compression
```

## Comparing `nonebot_plugin_daily_task-0.1.2.tar` & `nonebot_plugin_daily_task-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-05-26 16:33:51.810140 nonebot_plugin_daily_task-0.1.2/LICENSE
--rw-r--r--   0        0        0     2436 2024-05-26 16:33:51.810140 nonebot_plugin_daily_task-0.1.2/README.md
--rw-r--r--   0        0        0    14893 2024-05-26 16:33:51.810140 nonebot_plugin_daily_task-0.1.2/nonebot_plugin_daily_task/__init__.py
--rw-r--r--   0        0        0      550 2024-05-26 16:33:51.810140 nonebot_plugin_daily_task-0.1.2/nonebot_plugin_daily_task/config.py
--rw-r--r--   0        0        0      402 2024-05-26 16:34:03.478137 nonebot_plugin_daily_task-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2436 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/README.md
+-rw-r--r--   0        0        0    14889 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/config.py
+-rw-r--r--   0        0        0      402 2024-05-27 12:05:20.116658 nonebot_plugin_daily_task-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_daily_task-0.1.2/LICENSE` & `nonebot_plugin_daily_task-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.2/README.md` & `nonebot_plugin_daily_task-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.2/nonebot_plugin_daily_task/__init__.py` & `nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                                  'start_date': start_date.isoformat(),
                                  'end_date': end_date})
         # 返回信息
         msg = MessageTemplate("任务已记录:\nid: {}\ntask: {}\nstart time: {}"
                               .format(user_id, job, start_date))
         await daily_add.send(msg)
         # 更新‘Status’数据库
-        await update_status_add(user_id=user_id)
+        await update_status_add(uid=user_id)
     else:
         await daily_add.finish("请在命令后加上要添加的任务..")
 
 
 # 查询'Task'数据库中的任务
 async def query_task(user_id: str, **kwargs):
     """查询指定user的任务"""
```

### Comparing `nonebot_plugin_daily_task-0.1.2/nonebot_plugin_daily_task/config.py` & `nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.2/PKG-INFO` & `nonebot_plugin_daily_task-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_daily_task
-Version: 0.1.2
+Version: 0.1.3
 Summary: 适用于Nonebot2的每日任务提醒插件
 Author-Email: WMGray <1466787434@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD041 -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.3 Summary:
 éç¨äºNonebot2çæ¯æ¥ä»»å¡æéæä»¶ Author-Email: WMGray
 <1466787434@qq.com> License: MIT Requires-Python: >=3.10 Description-Content-
 Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
 # nonebot-plugin-daily-task _â¨ NoneBot æ¯æ¥ä»»å¡æä»¶ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ nb plugin install nonebot-plugin-daily-task
```

