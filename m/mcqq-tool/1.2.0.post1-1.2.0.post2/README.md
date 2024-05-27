# Comparing `tmp/mcqq_tool-1.2.0.post1.tar.gz` & `tmp/mcqq_tool-1.2.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqq_tool-1.2.0.post1.tar", max compression
+gzip compressed data, was "mcqq_tool-1.2.0.post2.tar", max compression
```

## Comparing `mcqq_tool-1.2.0.post1.tar` & `mcqq_tool-1.2.0.post2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/LICENSE
--rw-r--r--   0        0        0      155 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/README.md
--rw-r--r--   0        0        0       19 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/__init__.py
--rw-r--r--   0        0        0     2116 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/config.py
--rw-r--r--   0        0        0      266 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/model.py
--rw-r--r--   0        0        0    14873 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/parse_qq_msg.py
--rw-r--r--   0        0        0     5174 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/rule.py
--rw-r--r--   0        0        0    10672 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/send_to_mc.py
--rw-r--r--   0        0        0     3257 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/mcqq_tool/send_to_qq.py
--rw-r--r--   0        0        0     1194 2024-05-25 11:15:07.060337 mcqq_tool-1.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 mcqq_tool-1.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/LICENSE
+-rw-r--r--   0        0        0      155 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/README.md
+-rw-r--r--   0        0        0       19 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/__init__.py
+-rw-r--r--   0        0        0     2116 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/config.py
+-rw-r--r--   0        0        0      266 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/model.py
+-rw-r--r--   0        0        0    14873 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/parse_qq_msg.py
+-rw-r--r--   0        0        0     5174 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/rule.py
+-rw-r--r--   0        0        0    10859 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/send_to_mc.py
+-rw-r--r--   0        0        0     3257 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/mcqq_tool/send_to_qq.py
+-rw-r--r--   0        0        0     1194 2024-05-27 11:13:25.425516 mcqq_tool-1.2.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 mcqq_tool-1.2.0.post2/PKG-INFO
```

### Comparing `mcqq_tool-1.2.0.post1/LICENSE` & `mcqq_tool-1.2.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.2.0.post1/mcqq_tool/config.py` & `mcqq_tool-1.2.0.post2/mcqq_tool/config.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.2.0.post1/mcqq_tool/parse_qq_msg.py` & `mcqq_tool-1.2.0.post2/mcqq_tool/parse_qq_msg.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.2.0.post1/mcqq_tool/rule.py` & `mcqq_tool-1.2.0.post2/mcqq_tool/rule.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.2.0.post1/mcqq_tool/send_to_mc.py` & `mcqq_tool-1.2.0.post2/mcqq_tool/send_to_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,46 +147,48 @@
             if is_cmd:
                 send_temp_result += f"命令：{command} "
 
                 if server_config.rcon_cmd and mc_bot.rcon:
                     if command_type == "title":
                         title, subtitle = command.split("\n") if "\n" in command else (command, "")
                         title_cmd = f'title @a title ["{title}"]'
-                        title_result = (await mc_bot.send_rcon_cmd(title_cmd))[0]
+                        title_result = (await mc_bot.send_rcon_cmd(command=title_cmd))[0]
                         if subtitle:
                             subtitle_cmd = f'title @a subtitle ["{subtitle}"]'
-                            title_result += (await mc_bot.send_rcon_cmd(subtitle_cmd))[0]
+                            title_result += (await mc_bot.send_rcon_cmd(command=subtitle_cmd))[0]
                         send_temp_result += f"结果：{title_result}"
                     elif command_type == "command":
-                        response = await mc_bot.send_rcon_cmd(command)
+                        response = await mc_bot.send_rcon_cmd(command=command)
                         send_temp_result += f"结果：{response[0]}\n"
                     else:
                         cmd = parse_qq_screen_cmd_to_rcon_model(command_type, command)
-                        response = await mc_bot.send_rcon_cmd(cmd)
+                        response = await mc_bot.send_rcon_cmd(command=cmd)
                         send_temp_result += f"结果：{response[0]}\n"
                 elif server_config.rcon_cmd and not mc_bot.rcon:
                     send_temp_result += "选择了Rcon发送命令，但无rcon可用，无法发送命令\n"
                 else:
                     if command_type == "title":
                         title, subtitle = command.split("\n") if "\n" in command else (command, "")
                         await mc_bot.send_title(title=title, subtitle=subtitle)
                     elif command_type == "action_bar":
                         await mc_bot.send_actionbar(message=command)
                     else:
                         await mc_bot.send_msg(message=command)
+                        send_temp_result += "结果：没有可用的命令发送，请检查Rcon或其他配置"
+                        continue
                     send_temp_result += "结果：成功\n"
 
             else:
                 send_temp_result += "消息："
 
                 if server_config.rcon_msg and mc_bot.rcon:
                     msg, text = await parse_qq_msg_to_rcon_model(bot=bot, event=event)
                     msg = msg.replace("'", '"')
                     send_temp_result += f"{text} "
-                    response = await mc_bot.send_rcon_cmd(f"tellraw @a {msg}")
+                    response = await mc_bot.send_rcon_cmd(command=f"tellraw @a {msg}")
                     send_temp_result += f"结果：{response[0]}\n"
 
                 elif server_config.rcon_msg and not mc_bot.rcon:
                     send_temp_result += "选择了Rcon发送消息，但无rcon未开启，无法发送消息\n"
 
                 else:
                     msg, text = await parse_qq_msg_to_base_model(bot=bot, event=event)
```

### Comparing `mcqq_tool-1.2.0.post1/mcqq_tool/send_to_qq.py` & `mcqq_tool-1.2.0.post2/mcqq_tool/send_to_qq.py`

 * *Files identical despite different names*

### Comparing `mcqq_tool-1.2.0.post1/pyproject.toml` & `mcqq_tool-1.2.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mcqq-tool"
-version = "1.2.0.post1"
+version = "1.2.0.post2"
 description = "MC_QQ工具包"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mcqq_tool-1.2.0.post1/PKG-INFO` & `mcqq_tool-1.2.0.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcqq-tool
-Version: 1.2.0.post1
+Version: 1.2.0.post2
 Summary: MC_QQ工具包
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

