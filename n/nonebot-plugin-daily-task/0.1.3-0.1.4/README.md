# Comparing `tmp/nonebot_plugin_daily_task-0.1.3.tar.gz` & `tmp/nonebot_plugin_daily_task-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_daily_task-0.1.3.tar", last modified: Mon May 27 12:05:20 2024, max compression
+gzip compressed data, was "nonebot_plugin_daily_task-0.1.4.tar", last modified: Mon May 27 12:38:37 2024, max compression
```

## Comparing `nonebot_plugin_daily_task-0.1.3.tar` & `nonebot_plugin_daily_task-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/LICENSE
--rw-r--r--   0        0        0     2436 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/README.md
--rw-r--r--   0        0        0    14889 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/__init__.py
--rw-r--r--   0        0        0      550 2024-05-27 12:05:09.276730 nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/config.py
--rw-r--r--   0        0        0      402 2024-05-27 12:05:20.116658 nonebot_plugin_daily_task-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2418 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/README.md
+-rw-r--r--   0        0        0    14915 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/__init__.py
+-rw-r--r--   0        0        0      546 2024-05-27 12:38:27.514226 nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/config.py
+-rw-r--r--   0        0        0      402 2024-05-27 12:38:37.018224 nonebot_plugin_daily_task-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 nonebot_plugin_daily_task-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_daily_task-0.1.3/LICENSE` & `nonebot_plugin_daily_task-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_daily_task-0.1.3/README.md` & `nonebot_plugin_daily_task-0.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 # nonebot-plugin-daily-task
 
 _✨ NoneBot 每日任务插件 ✨_
 
 
 <a href="https://github.com/WMGray/nonebot-plugin-daily-task/blob/master/LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+    <img src="https://img.shields.io/github/license/WMGray/nonebot-plugin-daily-task" alt="license">
 </a>
 <a href="https://pypi.org/project/nonebot-plugin-daily-task/">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-daily-task" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 💿 安装
 
@@ -60,9 +60,7 @@
 |  daily.del/d   |  删除每日任务  |    所有人    |
 | daily.modify/m |  修改每日任务  |    所有人    |
 | daily.query/q  |  查询每日任务  |    所有人    |
 | daily.finish/f |  完成每日任务  |    所有人    |
 | daily.start/s  |  启用每日任务  | SUPERUSER |
 | daily.stop/st  |  停用每日任务  | SUPERUSER |
 
-### 效果图
-
```

#### html2text {}

```diff
@@ -17,8 +17,8 @@
 æä»¤è¡¨ | æä»¤ | åè½ | æé | |:--------------:|:--------:|:---------:
 | | daily | æä»¶ç®ä» | ææäºº | | daily.help/h |
 æ¥çæä»¶å¸®å©ä¿¡æ¯ | ææäºº | | daily.add/a | æ·»å æ¯æ¥ä»»å¡ |
 ææäºº | | daily.del/d | å é¤æ¯æ¥ä»»å¡ | ææäºº | | daily.modify/m |
 ä¿®æ¹æ¯æ¥ä»»å¡ | ææäºº | | daily.query/q | æ¥è¯¢æ¯æ¥ä»»å¡ |
 ææäºº | | daily.finish/f | å®ææ¯æ¥ä»»å¡ | ææäºº | | daily.start/
 s | å¯ç¨æ¯æ¥ä»»å¡ | SUPERUSER | | daily.stop/st | åç¨æ¯æ¥ä»»å¡ |
-SUPERUSER | ### ææå¾
+SUPERUSER |
```

### Comparing `nonebot_plugin_daily_task-0.1.3/nonebot_plugin_daily_task/__init__.py` & `nonebot_plugin_daily_task-0.1.4/nonebot_plugin_daily_task/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # 插件信息
 __plugin_meta__ = PluginMetadata(
     name="Daily Task",
     description="这个插件可以帮助用户管理每日任务，包括添加任务、完成任务、查询任务等功能。",
     usage="帮助 daily.h daily.help",
     type="application",
-    homepage="{项目主页}",
+    homepage="https://github.com/WMGray/nonebot-plugin-daily-task/",
     # 发布必填。
     config=Config,
     # 插件配置项类，如无需配置可不填写。
     supported_adapters={"~onebot.v11"},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
@@ -39,15 +39,15 @@
 # 加载插件配置
 cfg = get_plugin_config(Config)
 driver = get_driver()
 db = None
 
 
 async def is_enable() -> bool:
-    return cfg.weather_plugin_enabled
+    return cfg.daily_task_enabled
 
 
 # 配置响应器组
 daily_group = CommandGroup(
     'daily',
     rule=to_me(),
     prefix_aliases=True,
@@ -364,15 +364,15 @@
     else:
         await daily_query.send("未指定User")
 
 
 @daily_start.handle()
 async def start_task(event: Event):
     """启动定时任务"""
-    cfg.weather_plugin_enabled = True
+    cfg.daily_task_enabled = True
     await _init_db()
     start_h, end_h = cfg.daily_task_start_hour, cfg.daily_task_end_hour
     interval_h = cfg.daily_task_interval_hour
     # 创建两个定时任务： 每日0点更新任务状态 & 每日10-22点每分钟提醒
     scheduler.add_job(update_status_add, "cron", hour=0)
     # scheduler.add_job(update_status_add, "cron", hour=f"{start_h}-{end_h}/{interval_h}"
     #                   , minute='*')
@@ -386,10 +386,10 @@
                           , minute='*', args=[user_id], id=user_id)
     await daily_start.finish("定时任务已启动")
 
 
 @daily_stop.handle()
 async def stop_task(event: Event):
     """停止定时任务"""
-    cfg.weather_plugin_enabled = False
+    cfg.daily_task_enabled = False
     scheduler.remove_all_jobs()
     await daily_stop.finish("定时任务已停止")
```

### Comparing `nonebot_plugin_daily_task-0.1.3/PKG-INFO` & `nonebot_plugin_daily_task-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_daily_task
-Version: 0.1.3
+Version: 0.1.4
 Summary: 适用于Nonebot2的每日任务提醒插件
 Author-Email: WMGray <1466787434@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD041 -->
@@ -16,18 +16,18 @@
 
 # nonebot-plugin-daily-task
 
 _✨ NoneBot 每日任务插件 ✨_
 
 
 <a href="https://github.com/WMGray/nonebot-plugin-daily-task/blob/master/LICENSE">
-    <img src="https://img.shields.io/github/license/owner/nonebot-plugin-template.svg" alt="license">
+    <img src="https://img.shields.io/github/license/WMGray/nonebot-plugin-daily-task" alt="license">
 </a>
 <a href="https://pypi.org/project/nonebot-plugin-daily-task/">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-template.svg" alt="pypi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-daily-task" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">
 
 </div>
 
 ## 💿 安装
 
@@ -69,9 +69,7 @@
 |  daily.del/d   |  删除每日任务  |    所有人    |
 | daily.modify/m |  修改每日任务  |    所有人    |
 | daily.query/q  |  查询每日任务  |    所有人    |
 | daily.finish/f |  完成每日任务  |    所有人    |
 | daily.start/s  |  启用每日任务  | SUPERUSER |
 | daily.stop/st  |  停用每日任务  | SUPERUSER |
 
-### 效果图
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_daily_task Version: 0.1.4 Summary:
 éç¨äºNonebot2çæ¯æ¥ä»»å¡æéæä»¶ Author-Email: WMGray
 <1466787434@qq.com> License: MIT Requires-Python: >=3.10 Description-Content-
 Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
 # nonebot-plugin-daily-task _â¨ NoneBot æ¯æ¥ä»»å¡æä»¶ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ nb plugin install nonebot-plugin-daily-task
@@ -21,8 +21,8 @@
 æä»¤è¡¨ | æä»¤ | åè½ | æé | |:--------------:|:--------:|:---------:
 | | daily | æä»¶ç®ä» | ææäºº | | daily.help/h |
 æ¥çæä»¶å¸®å©ä¿¡æ¯ | ææäºº | | daily.add/a | æ·»å æ¯æ¥ä»»å¡ |
 ææäºº | | daily.del/d | å é¤æ¯æ¥ä»»å¡ | ææäºº | | daily.modify/m |
 ä¿®æ¹æ¯æ¥ä»»å¡ | ææäºº | | daily.query/q | æ¥è¯¢æ¯æ¥ä»»å¡ |
 ææäºº | | daily.finish/f | å®ææ¯æ¥ä»»å¡ | ææäºº | | daily.start/
 s | å¯ç¨æ¯æ¥ä»»å¡ | SUPERUSER | | daily.stop/st | åç¨æ¯æ¥ä»»å¡ |
-SUPERUSER | ### ææå¾
+SUPERUSER |
```

