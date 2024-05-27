# Comparing `tmp/aurum_hikari-0.1.5.4.tar.gz` & `tmp/aurum_hikari-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.5.4.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.5.5.tar", max compression
```

## Comparing `aurum_hikari-0.1.5.4.tar` & `aurum_hikari-0.1.5.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1080 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/LICENSE
--rw-r--r--   0        0        0     3510 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/README.md
--rw-r--r--   0        0        0      584 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/__init__.py
--rw-r--r--   0        0        0      382 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/__main__.py
--rw-r--r--   0        0        0      563 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/_about.py
--rw-r--r--   0        0        0      183 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/__init__.py
--rw-r--r--   0        0        0     9439 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/client.py
--rw-r--r--   0        0        0      720 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/client/integration.py
--rw-r--r--   0        0        0      366 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2324 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/message_command.py
--rw-r--r--   0        0        0     5767 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2720 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-25 23:35:21.793463 aurum_hikari-0.1.5.4/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/__init__.py
--rw-r--r--   0        0        0      312 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     1724 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_integration.py
--rw-r--r--   0        0        0     3462 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     8642 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     5738 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/utils/commands.py
--rw-r--r--   0        0        0      226 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/internal/version.py
--rw-r--r--   0        0        0      360 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/localized.py
--rw-r--r--   0        0        0      479 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-25 23:35:21.797463 aurum_hikari-0.1.5.4/aurum/types.py
--rw-r--r--   0        0        0     2360 2024-05-25 23:35:30.857595 aurum_hikari-0.1.5.4/pyproject.toml
--rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/LICENSE
+-rw-r--r--   0        0        0     3510 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/README.md
+-rw-r--r--   0        0        0      584 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/__main__.py
+-rw-r--r--   0        0        0      563 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/_about.py
+-rw-r--r--   0        0        0      183 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/client/__init__.py
+-rw-r--r--   0        0        0     9579 2024-05-27 16:39:03.307608 aurum_hikari-0.1.5.5/aurum/client/client.py
+-rw-r--r--   0        0        0      720 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/client/integration.py
+-rw-r--r--   0        0        0      366 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2324 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5767 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2720 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     1724 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_integration.py
+-rw-r--r--   0        0        0     3462 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     8895 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     5738 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      226 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/internal/version.py
+-rw-r--r--   0        0        0      360 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      479 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-27 16:39:03.311608 aurum_hikari-0.1.5.5/aurum/types.py
+-rw-r--r--   0        0        0     2360 2024-05-27 16:39:12.007720 aurum_hikari-0.1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.5/PKG-INFO
```

### Comparing `aurum_hikari-0.1.5.4/LICENSE` & `aurum_hikari-0.1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/README.md` & `aurum_hikari-0.1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/__init__.py` & `aurum_hikari-0.1.5.5/aurum/__init__.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/_about.py` & `aurum_hikari-0.1.5.5/aurum/_about.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 import typing
 
 from aurum.internal.version import Version
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
-__version_tuple__: Version = Version(0, 1, 5, 4)
+__version_tuple__: Version = Version(0, 1, 5, 5)
 __version__: str = str(__version_tuple__)
```

### Comparing `aurum_hikari-0.1.5.4/aurum/client/client.py` & `aurum_hikari-0.1.5.5/aurum/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,24 @@
             will be used, which will pass all functions and return the key.
         integrations: (Sequence[IClientIntegration]): A list of integrations for client.
         sync_commands (SyncCommandFlag): An optional SyncCommandsFlag enum value, indicating how to handle command synchronization.
         ignore_l10n (bool): An optional flag. If `True`, the client will not emit a warning when a localization provider is not provided.
         ignore_unknown_interactions (bool): An optional flag that, if set to `True`, will disable the warning message for unknown interactions.
     """
 
-    # __slots__ was removed, because integrations
-    # integrations add a new variables to a class and __slots__ broke this conception
-    # idk how bad is this
+    __slots__: Sequence[str] = (
+        "__logger",
+        "_starting_tasks",
+        "_sync_commands",
+        "_ignore_unknown_interactions",
+        "l10n",
+        "bot",
+        "commands",
+        "plugins",
+    )
 
     def __init__(
         self,
         bot: BotT,
         *,
         l10n: LocalizationProviderInterface | None = None,
         integrations: Sequence[IClientIntegration] = (),
@@ -178,22 +185,26 @@
                 for option in options or ():
                     arguments[option.name] = context.resolve_command_argument(option)
             callback: Callable[..., Coroutine[None, None, typing.Any]] = getattr(
                 command, "callback"
             )
             if isinstance(command, SlashCommand):
                 await callback(context, **arguments)
+                return
             await callback(parent_command, context, **arguments)
+            return
         if interaction.command_type is CommandType.MESSAGE:
             assert isinstance(command, MessageCommand)
             assert interaction.resolved
             await command.callback(
                 context,
                 list(interaction.resolved.messages.values())[0],
             )
+            return
         if interaction.command_type is CommandType.USER:
             assert isinstance(command, UserCommand)
             assert interaction.resolved
             await command.callback(
                 context,
                 list(interaction.resolved.users.values())[0],
             )
+            return
```

### Comparing `aurum_hikari-0.1.5.4/aurum/client/integration.py` & `aurum_hikari-0.1.5.5/aurum/client/integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.5.5/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/commands/message_command.py` & `aurum_hikari-0.1.5.5/aurum/commands/message_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/commands/slash_command.py` & `aurum_hikari-0.1.5.5/aurum/commands/slash_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/commands/sub_command.py` & `aurum_hikari-0.1.5.5/aurum/commands/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/commands/user_command.py` & `aurum_hikari-0.1.5.5/aurum/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_integration.py` & `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.5.5/aurum/ext/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.5.5/aurum/interactions/interaction_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from hikari.snowflakes import Snowflake
 from hikari.undefined import UNDEFINED
 
 if typing.TYPE_CHECKING:
     from collections.abc import Sequence
 
     from hikari.api import ComponentBuilder
+    from hikari.channels import PartialChannel
     from hikari.embeds import Embed
     from hikari.files import Resourceish
-    from hikari.guilds import PartialRole
+    from hikari.guilds import GatewayGuild, PartialRole
     from hikari.interactions import (
         CommandInteraction,
         CommandInteractionOption,
         ComponentInteraction,
         InteractionMember,
     )
     from hikari.messages import Message
@@ -55,29 +56,37 @@
         return self.interaction.user
 
     @property
     def member(self) -> InteractionMember | None:
         """Member of the interaction"""
         return self.interaction.member
 
+    @property
+    def guild(self) -> GatewayGuild | None:
+        return self.interaction.get_guild()
+
+    @property
+    def channel(self) -> PartialChannel | None:
+        return self.interaction.get_channel()
+
     async def defer(
         self, flags: MessageFlag = MessageFlag.NONE, *, ephemeral: bool = False
     ) -> None:
         """Create a deferred response to the interaction.
 
         Note:
             The interaction will be available in the next 15 minutes.
 
         Arguments:
             flags (MessageFlag): An optional flags for response.
             ephemeral (bool): An optional flag to create ephemeral response.
                 Ephemeral messages that only the author of the interaction can see.
                 They are similar to Clyde's messages.
         """
-        if flags and ephemeral:
+        if ephemeral:
             flags |= MessageFlag.EPHEMERAL
         return await self.bot.rest.create_interaction_response(
             interaction=self.interaction.id,
             token=self.interaction.token,
             flags=flags,
             response_type=ResponseType.DEFERRED_MESSAGE_CREATE,
         )
@@ -123,15 +132,15 @@
             user_mentions:
                 - Allows to ping users is set to `True`.
                 - A list of users that can be pinged in response.
             role_mentions:
                 - Allows to ping roles is set to `True`.
                 - A list of roles that can be pinged in response.
         """
-        if flags and ephemeral:
+        if ephemeral:
             flags |= MessageFlag.EPHEMERAL
         return await self.bot.rest.create_interaction_response(
             interaction=self.interaction.id,
             response_type=ResponseType.MESSAGE_CREATE,
             token=self.interaction.token,
             content=content,
             flags=flags,
```

### Comparing `aurum_hikari-0.1.5.4/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.5.5/aurum/internal/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.5.5/aurum/internal/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.5.5/aurum/internal/commands/context_menu_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/internal/utils/commands.py` & `aurum_hikari-0.1.5.5/aurum/internal/utils/commands.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.5.5/aurum/l10n/localization_provider_interface.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/aurum/options/option.py` & `aurum_hikari-0.1.5.5/aurum/options/option.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.4/pyproject.toml` & `aurum_hikari-0.1.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "v0.1.5.4"
+version = "v0.1.5.5"
 name = "aurum-hikari"
 authors = ["stefanlight8 <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible framework for handling commands and components with integrations."
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `aurum_hikari-0.1.5.4/PKG-INFO` & `aurum_hikari-0.1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.5.4
+Version: 0.1.5.5
 Summary: A flexible framework for handling commands and components with integrations.
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler,integrations
 Author: stefanlight8
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
```

