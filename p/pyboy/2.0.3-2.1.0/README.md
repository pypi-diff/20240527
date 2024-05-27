# Comparing `tmp/pyboy-2.0.3.tar.gz` & `tmp/pyboy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboy-2.0.3.tar", last modified: Mon Apr 22 09:06:03 2024, max compression
+gzip compressed data, was "pyboy-2.1.0.tar", last modified: Mon May 27 08:02:17 2024, max compression
```

## Comparing `pyboy-2.0.3.tar` & `pyboy-2.1.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.796517 pyboy-2.0.3/
--rw-r--r--   0 runner     (501) staff       (20)     7558 2024-04-22 09:03:07.000000 pyboy-2.0.3/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-04-22 09:03:07.000000 pyboy-2.0.3/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    16861 2024-04-22 09:06:03.796041 pyboy-2.0.3/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6992 2024-04-22 09:03:07.000000 pyboy-2.0.3/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.763400 pyboy-2.0.3/pyboy/
--rw-r--r--   0 runner     (501) staff       (20)      263 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5607 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.770180 pyboy-2.0.3/pyboy/api/
--rw-r--r--   0 runner     (501) staff       (20)      362 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1002 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/constants.py
--rw-r--r--   0 runner     (501) staff       (20)      485 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/memory_scanner.pxd
--rw-r--r--   0 runner     (501) staff       (20)     7232 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/memory_scanner.py
--rw-r--r--   0 runner     (501) staff       (20)      712 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/screen.pxd
--rw-r--r--   0 runner     (501) staff       (20)     8247 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/screen.py
--rw-r--r--   0 runner     (501) staff       (20)      671 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/sprite.pxd
--rw-r--r--   0 runner     (501) staff       (20)     7340 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/sprite.py
--rw-r--r--   0 runner     (501) staff       (20)      730 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/tile.pxd
--rw-r--r--   0 runner     (501) staff       (20)     7322 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/tile.py
--rw-r--r--   0 runner     (501) staff       (20)      659 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/tilemap.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9462 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/api/tilemap.py
--rw-r--r--   0 runner     (501) staff       (20)     9927 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.777748 pyboy-2.0.3/pyboy/core/
--rw-r--r--   0 runner     (501) staff       (20)       98 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      293 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/bootrom.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1282 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/bootrom.py
--rw-r--r--   0 runner     (501) staff       (20)      256 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/bootrom_cgb.bin
--rw-r--r--   0 runner     (501) staff       (20)      256 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/bootrom_dmg.bin
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.782360 pyboy-2.0.3/pyboy/core/cartridge/
--rw-r--r--   0 runner     (501) staff       (20)      261 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1359 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/base_mbc.pxd
--rw-r--r--   0 runner     (501) staff       (20)     5752 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/base_mbc.py
--rw-r--r--   0 runner     (501) staff       (20)      597 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/cartridge.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/cartridge.py
--rw-r--r--   0 runner     (501) staff       (20)      387 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc1.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3279 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc1.py
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc2.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1556 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc2.py
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc3.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2058 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc3.py
--rw-r--r--   0 runner     (501) staff       (20)      309 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc5.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1283 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/mbc5.py
--rw-r--r--   0 runner     (501) staff       (20)     1067 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/rtc.pxd
--rw-r--r--   0 runner     (501) staff       (20)     4108 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cartridge/rtc.py
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cpu.pxd
--rw-r--r--   0 runner     (501) staff       (20)     6852 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/cpu.py
--rw-r--r--   0 runner     (501) staff       (20)      658 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/interaction.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3586 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/interaction.py
--rw-r--r--   0 runner     (501) staff       (20)     8070 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/lcd.pxd
--rw-r--r--   0 runner     (501) staff       (20)    38273 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/lcd.py
--rw-r--r--   0 runner     (501) staff       (20)     2859 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/mb.pxd
--rw-r--r--   0 runner     (501) staff       (20)    26495 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/mb.py
--rw-r--r--   0 runner     (501) staff       (20)    51233 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/opcodes.pxd
--rw-r--r--   0 runner     (501) staff       (20)   141369 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/opcodes.py
--rw-r--r--   0 runner     (501) staff       (20)    43681 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/opcodes_gen.py
--rw-r--r--   0 runner     (501) staff       (20)      656 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/ram.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2412 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/ram.py
--rw-r--r--   0 runner     (501) staff       (20)     7670 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/sound.pxd
--rw-r--r--   0 runner     (501) staff       (20)    25955 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/sound.py
--rw-r--r--   0 runner     (501) staff       (20)      774 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/timer.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2554 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/core/timer.py
--rw-r--r--   0 runner     (501) staff       (20)    32768 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/default_rom.gb
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.783664 pyboy-2.0.3/pyboy/logging/
--rw-r--r--   0 runner     (501) staff       (20)      961 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/logging/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      581 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/logging/_logging.py
--rw-r--r--   0 runner     (501) staff       (20)      376 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/logging/logging.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2933 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/logging/logging.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.794657 pyboy-2.0.3/pyboy/plugins/
--rw-r--r--   0 runner     (501) staff       (20)      581 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      242 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/auto_pause.pxd
--rw-r--r--   0 runner     (501) staff       (20)      674 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/auto_pause.py
--rw-r--r--   0 runner     (501) staff       (20)     2101 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/base_plugin.pxd
--rw-r--r--   0 runner     (501) staff       (20)    10172 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/base_plugin.py
--rw-r--r--   0 runner     (501) staff       (20)     4407 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/debug.pxd
--rw-r--r--   0 runner     (501) staff       (20)    30310 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/debug.py
--rw-r--r--   0 runner     (501) staff       (20)      297 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/debug_prompt.pxd
--rw-r--r--   0 runner     (501) staff       (20)     4186 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/debug_prompt.py
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/disable_input.pxd
--rw-r--r--   0 runner     (501) staff       (20)      412 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/disable_input.py
--rw-r--r--   0 runner     (501) staff       (20)     6490 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/font.txt
--rw-r--r--   0 runner     (501) staff       (20)      449 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_kirby_dream_land.pxd
--rw-r--r--   0 runner     (501) staff       (20)     5710 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_kirby_dream_land.py
--rw-r--r--   0 runner     (501) staff       (20)      311 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_pokemon_gen1.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3260 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_pokemon_gen1.py
--rw-r--r--   0 runner     (501) staff       (20)      706 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_super_mario_land.pxd
--rw-r--r--   0 runner     (501) staff       (20)    19749 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_super_mario_land.py
--rw-r--r--   0 runner     (501) staff       (20)      634 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_tetris.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9363 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/game_wrapper_tetris.py
--rw-r--r--   0 runner     (501) staff       (20)     2872 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/manager.pxd
--rw-r--r--   0 runner     (501) staff       (20)    12667 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/manager.py
--rw-r--r--   0 runner     (501) staff       (20)     6616 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/manager_gen.py
--rw-r--r--   0 runner     (501) staff       (20)      271 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/record_replay.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2115 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/record_replay.py
--rw-r--r--   0 runner     (501) staff       (20)     1835 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/rewind.pxd
--rw-r--r--   0 runner     (501) staff       (20)    10604 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/rewind.py
--rw-r--r--   0 runner     (501) staff       (20)      277 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/screen_recorder.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2253 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/screen_recorder.py
--rw-r--r--   0 runner     (501) staff       (20)      249 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/screenshot_recorder.pxd
--rw-r--r--   0 runner     (501) staff       (20)     1216 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/screenshot_recorder.py
--rw-r--r--   0 runner     (501) staff       (20)      232 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_null.pxd
--rw-r--r--   0 runner     (501) staff       (20)      841 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_null.py
--rw-r--r--   0 runner     (501) staff       (20)      843 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_open_gl.pxd
--rw-r--r--   0 runner     (501) staff       (20)     6541 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_open_gl.py
--rw-r--r--   0 runner     (501) staff       (20)      740 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_sdl2.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9568 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/plugins/window_sdl2.py
--rw-r--r--   0 runner     (501) staff       (20)     3044 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/pyboy.pxd
--rw-r--r--   0 runner     (501) staff       (20)    65456 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/pyboy.py
--rw-r--r--   0 runner     (501) staff       (20)     1881 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/utils.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9482 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyboy/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-22 09:06:03.795011 pyboy-2.0.3/pyboy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    16861 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2906 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        7 2024-04-22 09:06:03.000000 pyboy-2.0.3/pyboy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2018 2024-04-22 09:03:07.000000 pyboy-2.0.3/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-04-22 09:06:03.796596 pyboy-2.0.3/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3774 2024-04-22 09:03:07.000000 pyboy-2.0.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.774437 pyboy-2.1.0/
+-rw-r--r--   0 runner     (501) staff       (20)     7558 2024-05-27 07:59:21.000000 pyboy-2.1.0/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-27 07:59:21.000000 pyboy-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    16450 2024-05-27 08:02:17.774078 pyboy-2.1.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2024-05-27 07:59:21.000000 pyboy-2.1.0/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.731816 pyboy-2.1.0/pyboy/
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5608 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.739929 pyboy-2.1.0/pyboy/api/
+-rw-r--r--   0 runner     (501) staff       (20)      362 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1002 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/constants.py
+-rw-r--r--   0 runner     (501) staff       (20)      485 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/memory_scanner.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     7232 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/memory_scanner.py
+-rw-r--r--   0 runner     (501) staff       (20)      712 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/screen.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     8247 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/screen.py
+-rw-r--r--   0 runner     (501) staff       (20)      671 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/sprite.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     7340 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/sprite.py
+-rw-r--r--   0 runner     (501) staff       (20)      730 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/tile.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     7322 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/tile.py
+-rw-r--r--   0 runner     (501) staff       (20)      659 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/tilemap.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9462 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/api/tilemap.py
+-rw-r--r--   0 runner     (501) staff       (20)    10260 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.747536 pyboy-2.1.0/pyboy/core/
+-rw-r--r--   0 runner     (501) staff       (20)       98 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      293 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/bootrom.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/bootrom.py
+-rw-r--r--   0 runner     (501) staff       (20)      256 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/bootrom_cgb.bin
+-rw-r--r--   0 runner     (501) staff       (20)      256 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/bootrom_dmg.bin
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.752718 pyboy-2.1.0/pyboy/core/cartridge/
+-rw-r--r--   0 runner     (501) staff       (20)      261 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1359 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/base_mbc.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     5752 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/base_mbc.py
+-rw-r--r--   0 runner     (501) staff       (20)      597 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/cartridge.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/cartridge.py
+-rw-r--r--   0 runner     (501) staff       (20)      387 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc1.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3279 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc1.py
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc2.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1556 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc2.py
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc3.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2202 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc3.py
+-rw-r--r--   0 runner     (501) staff       (20)      309 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc5.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1283 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/mbc5.py
+-rw-r--r--   0 runner     (501) staff       (20)     1090 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/rtc.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4261 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cartridge/rtc.py
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cpu.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     6852 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/cpu.py
+-rw-r--r--   0 runner     (501) staff       (20)      658 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/interaction.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3586 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/interaction.py
+-rw-r--r--   0 runner     (501) staff       (20)     8070 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/lcd.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    38273 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/lcd.py
+-rw-r--r--   0 runner     (501) staff       (20)     2859 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/mb.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    26495 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/mb.py
+-rw-r--r--   0 runner     (501) staff       (20)    51233 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/opcodes.pxd
+-rw-r--r--   0 runner     (501) staff       (20)   141369 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/opcodes.py
+-rw-r--r--   0 runner     (501) staff       (20)    43681 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/opcodes_gen.py
+-rw-r--r--   0 runner     (501) staff       (20)      656 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/ram.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2412 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/ram.py
+-rw-r--r--   0 runner     (501) staff       (20)     7670 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/sound.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    25955 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/sound.py
+-rw-r--r--   0 runner     (501) staff       (20)      774 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/timer.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2554 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/core/timer.py
+-rw-r--r--   0 runner     (501) staff       (20)    32768 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/default_rom.gb
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.753446 pyboy-2.1.0/pyboy/logging/
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/logging/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      581 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/logging/_logging.py
+-rw-r--r--   0 runner     (501) staff       (20)      376 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/logging/logging.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2933 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/logging/logging.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.773068 pyboy-2.1.0/pyboy/plugins/
+-rw-r--r--   0 runner     (501) staff       (20)      581 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      242 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/auto_pause.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      674 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/auto_pause.py
+-rw-r--r--   0 runner     (501) staff       (20)     2101 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/base_plugin.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    10110 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/base_plugin.py
+-rw-r--r--   0 runner     (501) staff       (20)     4407 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/debug.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    30310 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/debug.py
+-rw-r--r--   0 runner     (501) staff       (20)      297 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/debug_prompt.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4186 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/debug_prompt.py
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/disable_input.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      412 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/disable_input.py
+-rw-r--r--   0 runner     (501) staff       (20)     6490 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/font.txt
+-rw-r--r--   0 runner     (501) staff       (20)      449 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_kirby_dream_land.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     5549 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_kirby_dream_land.py
+-rw-r--r--   0 runner     (501) staff       (20)      311 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_pokemon_gen1.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3230 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_pokemon_gen1.py
+-rw-r--r--   0 runner     (501) staff       (20)     2168 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_pokemon_pinball.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    48737 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_pokemon_pinball.py
+-rw-r--r--   0 runner     (501) staff       (20)      706 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_super_mario_land.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    19588 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_super_mario_land.py
+-rw-r--r--   0 runner     (501) staff       (20)      634 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_tetris.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9241 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/game_wrapper_tetris.py
+-rw-r--r--   0 runner     (501) staff       (20)     3076 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/manager.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    13560 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/manager.py
+-rw-r--r--   0 runner     (501) staff       (20)     6649 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/manager_gen.py
+-rw-r--r--   0 runner     (501) staff       (20)      271 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/record_replay.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2115 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/record_replay.py
+-rw-r--r--   0 runner     (501) staff       (20)     1835 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/rewind.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    10604 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/rewind.py
+-rw-r--r--   0 runner     (501) staff       (20)      277 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/screen_recorder.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2253 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/screen_recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)      249 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/screenshot_recorder.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1216 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/screenshot_recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)      232 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_null.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      841 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_null.py
+-rw-r--r--   0 runner     (501) staff       (20)      843 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_open_gl.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     6541 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_open_gl.py
+-rw-r--r--   0 runner     (501) staff       (20)      740 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_sdl2.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9568 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/plugins/window_sdl2.py
+-rw-r--r--   0 runner     (501) staff       (20)     3044 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/pyboy.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    67269 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/pyboy.py
+-rw-r--r--   0 runner     (501) staff       (20)     1881 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/utils.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9482 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyboy/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-27 08:02:17.773296 pyboy-2.1.0/pyboy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    16450 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2999 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        7 2024-05-27 08:02:17.000000 pyboy-2.1.0/pyboy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2018 2024-05-27 07:59:21.000000 pyboy-2.1.0/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-27 08:02:17.774508 pyboy-2.1.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2024-05-27 07:59:21.000000 pyboy-2.1.0/setup.py
```

### Comparing `pyboy-2.0.3/LICENSE.md` & `pyboy-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/PKG-INFO` & `pyboy-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboy
-Version: 2.0.3
+Version: 2.1.0
 Summary: Game Boy emulator written in Python
 Author-email: Mads Ynddal <mads@ynddal.dk>
 License: GNU Lesser General Public License
         =================================
         
         _Version 3, 29 June 2007_
         _Copyright © 2007 Free Software Foundation, Inc. &lt;<http://fsf.org/>&gt;_
@@ -249,22 +249,14 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
-> [!WARNING]
-> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
->
-> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
-> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
->
-> If you're able to get in contact with PyPI, then please help us get this resolved!
-
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

### Comparing `pyboy-2.0.3/README.md` & `pyboy-2.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -58,22 +58,14 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
-> [!WARNING]
-> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
->
-> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
-> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
->
-> If you're able to get in contact with PyPI, then please help us get this resolved!
-
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

#### html2text {}

```diff
@@ -4,26 +4,21 @@
 584149554132418570?style=for-the-badge&logo=Discord&label=PyBoy)](https://
 discord.gg/Zrf2nyH)
          _T_r_a_i_n_ _R_L_ _a_g_e_n_t_s_ _t_o_ _p_l_a_y_ _P_o_k_e_m_o_n_ _R_e_d            _R_e_w_i_n_d_ _a_n_y_ _g_a_m_e
                       _[_W_a_t_c_h_ _t_h_e_ _v_i_d_e_o_]            [extras/README/5.gif]
    Play the classics       _C_r_e_a_t_e_ _y_o_u_r_ _o_w_n_ _A_I   _B_e_a_t_ _w_o_r_l_d_ _r_e_c_o_r_d_s_ _w_i_t_h_ _A_I
 [extras/README/1.gif]    [extras/README/6.gif]     [extras/README/7.gif]
 Getting Started =============== The instructions are simple: ```sh $ pip
-install pyboy ``` > [!WARNING] > **If you're having issues on Windows, try this
-instead:** `pip install pyboy==2.0.0 pillow` > > PyPI (who maintains `pip
-install`) has stopped processing support tickets, and we've been unable to
-deploy > a fix for over a month now. Follow this thread for status: https://
-github.com/pypi/support/issues/3757 > > If you're able to get in contact with
-PyPI, then please help us get this resolved! For details, see [installation
-instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation). Now you're
-ready! Either use PyBoy directly from the terminal ```sh $ pyboy game_rom.gb
-``` Or use it in your Python scripts: ```python from pyboy import PyBoy pyboy =
-PyBoy('game_rom.gb') while pyboy.tick(): pass pyboy.stop() ``` The API =======
-If you are looking to make a bot or AI, then these resources are a good place
-to start: * [PyBoy API Documentation](https://baekalfen.github.io/PyBoy/
+install pyboy ``` For details, see [installation instructions](https://
+github.com/Baekalfen/PyBoy/wiki/Installation). Now you're ready! Either use
+PyBoy directly from the terminal ```sh $ pyboy game_rom.gb ``` Or use it in
+your Python scripts: ```python from pyboy import PyBoy pyboy = PyBoy
+('game_rom.gb') while pyboy.tick(): pass pyboy.stop() ``` The API ======= If
+you are looking to make a bot or AI, then these resources are a good place to
+start: * [PyBoy API Documentation](https://baekalfen.github.io/PyBoy/
 index.html) * [Wiki Pages](https://github.com/Baekalfen/PyBoy/wiki/) * [Using
 PyBoy with Gym](https://github.com/Baekalfen/PyBoy/wiki/Using-PyBoy-with-Gym) *
 [Example: Kirby](https://github.com/Baekalfen/PyBoy/wiki/Example-Kirby) *
 [Example: Tetris](https://github.com/Baekalfen/PyBoy/wiki/Example-Tetris) *
 [Example: Super Mario Land](https://github.com/Baekalfen/PyBoy/wiki/Example-
 Super-Mario-Land) * [Code Examples](https://github.com/Baekalfen/PyBoy/tree/
 master/extras/examples) * [Discord](https://discord.gg/Zrf2nyH) When the
```

### Comparing `pyboy-2.0.3/pyboy/__main__.py` & `pyboy-2.1.0/pyboy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 )
 parser.add_argument("ROM", type=valid_file_path, help="Path to a Game Boy compatible ROM file")
 parser.add_argument("-b", "--bootrom", dest="bootrom", type=valid_file_path, help="Path to a boot-ROM file")
 parser.add_argument(
     "--log-level",
     default=defaults["log_level"],
     type=str,
-    choices=["ERROR", "WARNING", "INFO", "DEBUG", "DISABLE"],
+    choices=["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"],
     help="Set logging level"
 )
 parser.add_argument(
     "--color-palette",
     type=color_tuple,
     default=defaults["color_palette"],
     help=('Four comma seperated, hexadecimal, RGB values for colors (i.e. "FFFFFF,999999,555555,000000")')
```

### Comparing `pyboy-2.0.3/pyboy/api/constants.py` & `pyboy-2.1.0/pyboy/api/constants.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/memory_scanner.py` & `pyboy-2.1.0/pyboy/api/memory_scanner.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/screen.pxd` & `pyboy-2.1.0/pyboy/api/screen.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/screen.py` & `pyboy-2.1.0/pyboy/api/screen.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/sprite.pxd` & `pyboy-2.1.0/pyboy/api/sprite.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/sprite.py` & `pyboy-2.1.0/pyboy/api/sprite.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/tile.pxd` & `pyboy-2.1.0/pyboy/api/tile.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/tile.py` & `pyboy-2.1.0/pyboy/api/tile.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/tilemap.pxd` & `pyboy-2.1.0/pyboy/api/tilemap.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/api/tilemap.py` & `pyboy-2.1.0/pyboy/api/tilemap.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/conftest.py` & `pyboy-2.1.0/pyboy/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,14 +103,19 @@
 
 
 @pytest.fixture(scope="session")
 def supermarioland_rom(secrets):
     return locate_sha256(b"470d6c45c9bcf7f0397d00c1ae6de727c63dd471049c8eedbefdc540ceea80b4")
 
 
+@pytest.fixture(scope="session")
+def pokemon_pinball_rom(secrets):
+    return locate_sha256(b"7672001d4710272009df6a41e3cbada65decd56e0eb2f185cb3d59c08d33ea0e")
+
+
 tetris_game_area = np.array([
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
     [47, 47, 47, 130, 130, 47, 47, 47, 47, 47],
     [47, 47, 47, 47, 130, 130, 47, 47, 47, 47],
@@ -127,15 +132,15 @@
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
     [47, 47, 47, 47, 47, 47, 47, 47, 47, 47],
 ],
                             dtype=np.uint32)
 
 
 @pytest.fixture(autouse=True)
-def doctest_fixtures(doctest_namespace, default_rom, default_rom_cgb, supermarioland_rom):
+def doctest_fixtures(doctest_namespace, default_rom, default_rom_cgb, supermarioland_rom, pokemon_pinball_rom):
     pyboy = PyBoy(default_rom, window="null", symbols="extras/default_rom/default_rom.sym")
     pyboy_cgb = PyBoy(default_rom_cgb, window="null", symbols="extras/default_rom/default_rom_cgb.sym")
 
     def mock_PyBoy(filename, *args, **kwargs):
         if not os.path.isfile(filename):
             filename = default_rom
         kwargs.pop("window", None)
@@ -143,23 +148,25 @@
 
     # We mock get_sprite_by_tile_identifier as default_rom doesn't use sprites
     with mock.patch("pyboy.PyBoy.get_sprite_by_tile_identifier", return_value=[[0, 2, 4], []]), \
         mock.patch("pyboy.PyBoy.game_area_collision", return_value=np.zeros(shape=(10,9), dtype=np.uint32)), \
         mock.patch("pyboy.PyBoy.game_area", return_value=tetris_game_area), \
         mock.patch("pyboy.PyBoy.load_state", return_value=None), \
         mock.patch("pyboy.PyBoy.stop", return_value=None), \
+        mock.patch("pyboy.PyBoy.rtc_lock_experimental", return_value=None), \
         mock.patch("PIL.Image.Image.show", return_value=None):
 
         pyboy.set_emulation_speed(0)
         pyboy.tick(10) # Just a few to get the logo up
         doctest_namespace["pyboy"] = pyboy
         doctest_namespace["pyboy_cgb"] = pyboy_cgb
         doctest_namespace["PyBoy"] = mock_PyBoy
         doctest_namespace["newline"] = "\n"
         doctest_namespace["supermarioland_rom"] = supermarioland_rom
+        doctest_namespace["pokemon_pinball_rom"] = pokemon_pinball_rom
 
         yield None
 
 
 # Code taken from PyTest is licensed with the following:
 # The MIT License (MIT)
```

### Comparing `pyboy-2.0.3/pyboy/core/bootrom.py` & `pyboy-2.1.0/pyboy/core/bootrom.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/base_mbc.pxd` & `pyboy-2.1.0/pyboy/core/cartridge/base_mbc.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/base_mbc.py` & `pyboy-2.1.0/pyboy/core/cartridge/base_mbc.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/cartridge.pxd` & `pyboy-2.1.0/pyboy/core/cartridge/cartridge.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/cartridge.py` & `pyboy-2.1.0/pyboy/core/cartridge/cartridge.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/mbc1.py` & `pyboy-2.1.0/pyboy/core/cartridge/mbc1.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/mbc2.py` & `pyboy-2.1.0/pyboy/core/cartridge/mbc2.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/mbc3.py` & `pyboy-2.1.0/pyboy/core/cartridge/mbc3.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,19 @@
                 # logger.debug("Unexpected command for MBC3: Address: 0x%0.4x, Value: 0x%0.2x", address, value)
         elif 0x2000 <= address < 0x4000:
             value &= 0b01111111
             if value == 0:
                 value = 1
             self.rombank_selected = value % self.external_rom_count
         elif 0x4000 <= address < 0x6000:
-            self.rambank_selected = value % self.external_ram_count
+            if 0x08 <= value <= 0x0C:
+                # RTC register select
+                self.rambank_selected = value
+            else:
+                self.rambank_selected = value % self.external_ram_count
         elif 0x6000 <= address < 0x8000:
             if self.rtc_enabled:
                 self.rtc.writecommand(value)
             # else:
             #     # NOTE: Pokemon Red/Blue will do this, but it can safely be ignored:
             #     # https://github.com/pret/pokered/issues/155
             #     logger.debug("RTC not present. Game tried to issue RTC command: 0x%0.4x, 0x%0.2x", address, value)
```

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/mbc5.py` & `pyboy-2.1.0/pyboy/core/cartridge/mbc5.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/rtc.pxd` & `pyboy-2.1.0/pyboy/core/cartridge/rtc.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 cdef Logger logger
 
 cdef class RTC:
     cdef str filename
     cdef bint latch_enabled
     cdef cython.double timezero
+    cdef bint timelock
     cdef uint64_t sec_latch
     cdef uint64_t min_latch
     cdef uint64_t hour_latch
     cdef uint64_t day_latch_low
     cdef uint64_t day_latch_high
     cdef uint64_t day_carry
     cdef uint64_t halt
```

### Comparing `pyboy-2.0.3/pyboy/core/cartridge/rtc.py` & `pyboy-2.1.0/pyboy/core/cartridge/rtc.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 logger = pyboy.logging.get_logger(__name__)
 
 
 class RTC:
     def __init__(self, filename):
         self.filename = filename + ".rtc"
 
+        self.timezero = time.time()
+        self.timelock = False
+        self.day_carry = 0
+        self.halt = 0
+
         if not os.path.exists(self.filename):
             logger.info("No RTC file found. Skipping.")
         else:
             with open(self.filename, "rb") as f:
                 self.load_state(IntIOWrapper(f), STATE_VERSION)
 
         self.latch_enabled = False
-
-        self.timezero = time.time()
-
         self.sec_latch = 0
         self.min_latch = 0
         self.hour_latch = 0
         self.day_latch_low = 0
         self.day_latch_high = 0
-        self.day_carry = 0
-        self.halt = 0
 
     def stop(self):
         with open(self.filename, "wb") as f:
             self.save_state(IntIOWrapper(f))
 
     def save_state(self, f):
         for b in struct.pack("f", self.timezero):
@@ -47,15 +47,18 @@
 
     def load_state(self, f, state_version):
         self.timezero = int(struct.unpack("f", bytes([f.read() for _ in range(4)]))[0])
         self.halt = f.read()
         self.day_carry = f.read()
 
     def latch_rtc(self):
-        t = time.time() - self.timezero
+        if self.timelock:
+            t = 0
+        else:
+            t = time.time() - self.timezero
         self.sec_latch = int(t % 60)
         self.min_latch = int((t//60) % 60)
         self.hour_latch = int((t//3600) % 24)
         days = int(t // 3600 // 24)
         self.day_latch_low = days & 0xFF
         self.day_latch_high = days >> 8
 
@@ -95,15 +98,18 @@
         else:
             logger.warning("Invalid RTC register: %0.4x", register)
 
     def setregister(self, register, value):
         if not self.latch_enabled:
             logger.debug("RTC: Set register, but nothing is latched! 0x%0.4x, 0x%0.2x", register, value)
 
-        t = time.time() - self.timezero
+        if self.timelock:
+            t = 0
+        else:
+            t = time.time() - self.timezero
         if register == 0x08:
             # TODO: What happens, when these value are larger than allowed?
             self.timezero = self.timezero - (t%60) - value
         elif register == 0x09:
             self.timezero = self.timezero - (t//60%60) - value
         elif register == 0x0A:
             self.timezero = self.timezero - (t//3600%24) - value
```

### Comparing `pyboy-2.0.3/pyboy/core/cpu.pxd` & `pyboy-2.1.0/pyboy/core/cpu.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/cpu.py` & `pyboy-2.1.0/pyboy/core/cpu.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/interaction.pxd` & `pyboy-2.1.0/pyboy/core/interaction.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/interaction.py` & `pyboy-2.1.0/pyboy/core/interaction.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/lcd.pxd` & `pyboy-2.1.0/pyboy/core/lcd.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/lcd.py` & `pyboy-2.1.0/pyboy/core/lcd.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/mb.pxd` & `pyboy-2.1.0/pyboy/core/mb.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/mb.py` & `pyboy-2.1.0/pyboy/core/mb.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/opcodes.pxd` & `pyboy-2.1.0/pyboy/core/opcodes.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/opcodes.py` & `pyboy-2.1.0/pyboy/core/opcodes.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/opcodes_gen.py` & `pyboy-2.1.0/pyboy/core/opcodes_gen.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/ram.pxd` & `pyboy-2.1.0/pyboy/core/ram.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/ram.py` & `pyboy-2.1.0/pyboy/core/ram.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/sound.pxd` & `pyboy-2.1.0/pyboy/core/sound.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/sound.py` & `pyboy-2.1.0/pyboy/core/sound.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/timer.pxd` & `pyboy-2.1.0/pyboy/core/timer.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/core/timer.py` & `pyboy-2.1.0/pyboy/core/timer.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/default_rom.gb` & `pyboy-2.1.0/pyboy/default_rom.gb`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/logging/__init__.py` & `pyboy-2.1.0/pyboy/logging/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         level = INFO
     elif level == "WARNING":
         level = WARNING
     elif level == "ERROR":
         level = ERROR
     elif level == "CRITICAL":
         level = CRITICAL
+    elif level == "DISABLE":
+        level = CRITICAL
     elif isinstance(level, int):
         pass
     else:
         raise ValueError(f"Invalid log level: {level}")
 
     _log_level = level
```

### Comparing `pyboy-2.0.3/pyboy/logging/_logging.py` & `pyboy-2.1.0/pyboy/logging/_logging.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/logging/logging.pyx` & `pyboy-2.1.0/pyboy/logging/logging.pyx`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/__init__.py` & `pyboy-2.1.0/pyboy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/auto_pause.py` & `pyboy-2.1.0/pyboy/plugins/auto_pause.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/base_plugin.pxd` & `pyboy-2.1.0/pyboy/plugins/base_plugin.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/base_plugin.py` & `pyboy-2.1.0/pyboy/plugins/base_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,31 +157,31 @@
         The state of the emulator is saved, and using `reset_game`, you can get back to this point of the game
         instantly.
 
         Args:
             timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
 
-        if not self.pyboy.frame_count == 0:
-            logger.warning("Calling start_game from an already running game. This might not work.")
         self.game_has_started = True
         self.saved_state.seek(0)
         self.pyboy.save_state(self.saved_state)
+        self._set_timer_div(timer_div)
 
     def reset_game(self, timer_div=None):
         """
         After calling `start_game`, you can call this method at any time to reset the game.
 
         Args:
             timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
 
         if self.game_has_started:
             self.saved_state.seek(0)
             self.pyboy.load_state(self.saved_state)
+            self._set_timer_div(timer_div)
             self.post_tick()
         else:
             logger.error("Tried to reset game, but it hasn't been started yet!")
 
     def game_over(self):
         """
         After calling `start_game`, you can call this method at any time to know if the game is over.
```

### Comparing `pyboy-2.0.3/pyboy/plugins/debug.pxd` & `pyboy-2.1.0/pyboy/plugins/debug.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/debug.py` & `pyboy-2.1.0/pyboy/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/debug_prompt.py` & `pyboy-2.1.0/pyboy/plugins/debug_prompt.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/font.txt` & `pyboy-2.1.0/pyboy/plugins/font.txt`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_kirby_dream_land.py` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_kirby_dream_land.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 
         The state of the emulator is saved, and using `reset_game`, you can get back to this point of the game
         instantly.
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
-        PyBoyGameWrapper.start_game(self, timer_div=timer_div)
 
         # Boot screen
         while True:
             self.pyboy.tick(1, False)
             if self.tilemap_background[0:3, 16] == [231, 224, 235]: # 'HAL' on the first screen
                 break
 
@@ -84,30 +83,25 @@
         # Skip level intro
         self.pyboy.button("start")
         self.pyboy.tick()
 
         # Wait for transition to finish (exit level intro screen, enter game)
         self.pyboy.tick(60, False)
 
-        self.saved_state.seek(0)
-        self.pyboy.save_state(self.saved_state)
-
-        self._set_timer_div(timer_div)
+        PyBoyGameWrapper.start_game(self, timer_div=timer_div)
 
     def reset_game(self, timer_div=None):
         """
         After calling `start_game`, you can call this method at any time to reset the game.
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
         PyBoyGameWrapper.reset_game(self, timer_div=timer_div)
 
-        self._set_timer_div(timer_div)
-
     def game_area(self):
         """
         Use this method to get a matrix of the "game area" of the screen.
 
         ```text
               0   1   2   3   4   5   6   7   8   9
           ____________________________________________________________________________________
```

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_pokemon_gen1.py` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_pokemon_gen1.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,16 @@
         scanline_parameters = self.pyboy.screen.tilemap_position_list
         WX = scanline_parameters[0][2]
         WY = scanline_parameters[0][3]
         self.use_background(WY != 0)
 
     def _get_screen_background_tilemap(self):
         ### SIMILAR TO CURRENT pyboy.game_wrapper.game_area(), BUT ONLY FOR BACKGROUND TILEMAP, SO NPC ARE SKIPPED
-        bsm = self.pyboy.botsupport_manager()
-        ((scx, scy), (wx, wy)) = bsm.screen().tilemap_position()
-        tilemap = np.array(bsm.tilemap_background[:, :])
+        ((scx, scy), (wx, wy)) = self.pyboy.screen.get_tilemap_position()
+        tilemap = np.array(self.pyboy.tilemap_background[:, :])
         return np.roll(np.roll(tilemap, -scy // 8, axis=0), -scx // 8, axis=1)[:18, :20]
 
     def _get_screen_walkable_matrix(self):
         walkable_tiles_indexes = []
         collision_ptr = self.pyboy.memory[0xD530] + (self.pyboy.memory[0xD531] << 8)
         tileset_type = self.pyboy.memory[0xFFD7]
         if tileset_type > 0:
```

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_super_mario_land.pxd` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_super_mario_land.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_super_mario_land.py` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_super_mario_land.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,14 @@
         ```
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
             * world_level (tuple): (world, level) to start the game from
             * unlock_level_select (bool): Unlock level selector menu
         """
-        PyBoyGameWrapper.start_game(self, timer_div=timer_div)
 
         if world_level is not None:
             self.set_world_level(*world_level)
 
         # Boot screen
         while True:
             self.pyboy.tick(1, False)
@@ -409,18 +408,15 @@
 
             # "MARIO" in the title bar and 0 is placed at score
             if self.tilemap_background[0:5, 0] == [278, 266, 283, 274, 280] and \
                self.tilemap_background[5, 1] == 256:
                 # Game has started
                 break
 
-        self.saved_state.seek(0)
-        self.pyboy.save_state(self.saved_state)
-
-        self._set_timer_div(timer_div)
+        PyBoyGameWrapper.start_game(self, timer_div=timer_div)
 
     def reset_game(self, timer_div=None):
         """
         After calling `start_game`, use this method to reset Mario to the beginning of `start_game`.
 
         If you want to reset to other worlds or levels of the game -- for example world 1-2 or 3-1 -- reset the entire
         emulator and provide the `world_level` on `start_game`.
@@ -433,16 +429,14 @@
         ```
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
         PyBoyGameWrapper.reset_game(self, timer_div=timer_div)
 
-        self._set_timer_div(timer_div)
-
     def game_area(self):
         """
         Use this method to get a matrix of the "game area" of the screen. This view is simplified to be perfect for
         machine learning applications.
 
         In Super Mario Land, this is almost the entire screen, expect for the top part showing the score, lives left
         and so on. These values can be found in the variables of this class.
```

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_tetris.pxd` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_tetris.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/game_wrapper_tetris.py` & `pyboy-2.1.0/pyboy/plugins/game_wrapper_tetris.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,43 +102,38 @@
 
         The state of the emulator is saved, and using `reset_game`, you can get back to this point of the game
         instantly.
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
-        # We don't supply the timer_div arg here, as it won't have the desired effect
-        PyBoyGameWrapper.start_game(self)
 
         # Boot screen
         while True:
             self.pyboy.tick(1, False)
             if self.tilemap_background[2:9, 14] == [89, 25, 21, 10, 34, 14, 27]: # '1PLAYER' on the first screen
                 break
 
         # Start game. Just press Start when the game allows us.
         for i in range(2):
             self.pyboy.button("start")
             self.pyboy.tick(7, False)
 
-        self.saved_state.seek(0)
-        self.pyboy.save_state(self.saved_state)
-
+        # We don't supply the timer_div arg here, as it won't have the desired effect
+        PyBoyGameWrapper.start_game(self)
         self.reset_game(timer_div=timer_div)
 
     def reset_game(self, timer_div=None):
         """
         After calling `start_game`, you can call this method at any time to reset the game.
 
         Kwargs:
             * timer_div (int): Replace timer's DIV register with this value. Use `None` to randomize.
         """
         PyBoyGameWrapper.reset_game(self, timer_div=timer_div)
-
-        self._set_timer_div(timer_div)
         self.pyboy.button("start")
         self.pyboy.tick(7, False)
 
     def game_area(self):
         """
         Use this method to get a matrix of the "game area" of the screen. This view is simplified to be perfect for
         machine learning applications.
```

### Comparing `pyboy-2.0.3/pyboy/plugins/manager.pxd` & `pyboy-2.1.0/pyboy/plugins/manager.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pyboy.plugins.screen_recorder cimport ScreenRecorder
 from pyboy.plugins.screenshot_recorder cimport ScreenshotRecorder
 from pyboy.plugins.debug_prompt cimport DebugPrompt
 from pyboy.plugins.game_wrapper_super_mario_land cimport GameWrapperSuperMarioLand
 from pyboy.plugins.game_wrapper_tetris cimport GameWrapperTetris
 from pyboy.plugins.game_wrapper_kirby_dream_land cimport GameWrapperKirbyDreamLand
 from pyboy.plugins.game_wrapper_pokemon_gen1 cimport GameWrapperPokemonGen1
+from pyboy.plugins.game_wrapper_pokemon_pinball cimport GameWrapperPokemonPinball
 # imports end
 
 
 cdef class PluginManager:
     cdef object pyboy
 
     cdef public PyBoyGameWrapper generic_game_wrapper
@@ -42,14 +43,15 @@
     cdef public ScreenRecorder screen_recorder
     cdef public ScreenshotRecorder screenshot_recorder
     cdef public DebugPrompt debug_prompt
     cdef public GameWrapperSuperMarioLand game_wrapper_super_mario_land
     cdef public GameWrapperTetris game_wrapper_tetris
     cdef public GameWrapperKirbyDreamLand game_wrapper_kirby_dream_land
     cdef public GameWrapperPokemonGen1 game_wrapper_pokemon_gen1
+    cdef public GameWrapperPokemonPinball game_wrapper_pokemon_pinball
     cdef bint window_sdl2_enabled
     cdef bint window_open_gl_enabled
     cdef bint window_null_enabled
     cdef bint debug_enabled
     cdef bint disable_input_enabled
     cdef bint auto_pause_enabled
     cdef bint record_replay_enabled
@@ -57,14 +59,15 @@
     cdef bint screen_recorder_enabled
     cdef bint screenshot_recorder_enabled
     cdef bint debug_prompt_enabled
     cdef bint game_wrapper_super_mario_land_enabled
     cdef bint game_wrapper_tetris_enabled
     cdef bint game_wrapper_kirby_dream_land_enabled
     cdef bint game_wrapper_pokemon_gen1_enabled
+    cdef bint game_wrapper_pokemon_pinball_enabled
     # plugin_cdef end
 
     cdef list handle_events(self, list) noexcept
     cpdef void post_tick(self) noexcept
     cdef void _post_tick_windows(self) noexcept
     cdef void frame_limiter(self, int) noexcept
     cdef str window_title(self) noexcept
```

### Comparing `pyboy-2.0.3/pyboy/plugins/manager.py` & `pyboy-2.1.0/pyboy/plugins/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pyboy.plugins.screen_recorder import ScreenRecorder # isort:skip
 from pyboy.plugins.screenshot_recorder import ScreenshotRecorder # isort:skip
 from pyboy.plugins.debug_prompt import DebugPrompt # isort:skip
 from pyboy.plugins.game_wrapper_super_mario_land import GameWrapperSuperMarioLand # isort:skip
 from pyboy.plugins.game_wrapper_tetris import GameWrapperTetris # isort:skip
 from pyboy.plugins.game_wrapper_kirby_dream_land import GameWrapperKirbyDreamLand # isort:skip
 from pyboy.plugins.game_wrapper_pokemon_gen1 import GameWrapperPokemonGen1 # isort:skip
+from pyboy.plugins.game_wrapper_pokemon_pinball import GameWrapperPokemonPinball # isort:skip
 # imports end
 
 
 def parser_arguments():
     # yield_plugins
     yield WindowSDL2.argv
     yield WindowOpenGL.argv
@@ -37,14 +38,15 @@
     yield ScreenRecorder.argv
     yield ScreenshotRecorder.argv
     yield DebugPrompt.argv
     yield GameWrapperSuperMarioLand.argv
     yield GameWrapperTetris.argv
     yield GameWrapperKirbyDreamLand.argv
     yield GameWrapperPokemonGen1.argv
+    yield GameWrapperPokemonPinball.argv
     # yield_plugins end
     pass
 
 
 class PluginManager:
     def __init__(self, pyboy, mb, pyboy_argv):
         self.pyboy = pyboy
@@ -78,22 +80,25 @@
         self.game_wrapper_super_mario_land_enabled = self.game_wrapper_super_mario_land.enabled()
         self.game_wrapper_tetris = GameWrapperTetris(pyboy, mb, pyboy_argv)
         self.game_wrapper_tetris_enabled = self.game_wrapper_tetris.enabled()
         self.game_wrapper_kirby_dream_land = GameWrapperKirbyDreamLand(pyboy, mb, pyboy_argv)
         self.game_wrapper_kirby_dream_land_enabled = self.game_wrapper_kirby_dream_land.enabled()
         self.game_wrapper_pokemon_gen1 = GameWrapperPokemonGen1(pyboy, mb, pyboy_argv)
         self.game_wrapper_pokemon_gen1_enabled = self.game_wrapper_pokemon_gen1.enabled()
+        self.game_wrapper_pokemon_pinball = GameWrapperPokemonPinball(pyboy, mb, pyboy_argv)
+        self.game_wrapper_pokemon_pinball_enabled = self.game_wrapper_pokemon_pinball.enabled()
         # plugins_enabled end
 
     def gamewrapper(self):
         # gamewrapper
         if self.game_wrapper_super_mario_land_enabled: return self.game_wrapper_super_mario_land
         if self.game_wrapper_tetris_enabled: return self.game_wrapper_tetris
         if self.game_wrapper_kirby_dream_land_enabled: return self.game_wrapper_kirby_dream_land
         if self.game_wrapper_pokemon_gen1_enabled: return self.game_wrapper_pokemon_gen1
+        if self.game_wrapper_pokemon_pinball_enabled: return self.game_wrapper_pokemon_pinball
         # gamewrapper end
         self.generic_game_wrapper_enabled = True
         return self.generic_game_wrapper
 
     def handle_events(self, events):
         # foreach windows events = [].handle_events(events)
         if self.window_sdl2_enabled:
@@ -124,14 +129,16 @@
             events = self.game_wrapper_super_mario_land.handle_events(events)
         if self.game_wrapper_tetris_enabled:
             events = self.game_wrapper_tetris.handle_events(events)
         if self.game_wrapper_kirby_dream_land_enabled:
             events = self.game_wrapper_kirby_dream_land.handle_events(events)
         if self.game_wrapper_pokemon_gen1_enabled:
             events = self.game_wrapper_pokemon_gen1.handle_events(events)
+        if self.game_wrapper_pokemon_pinball_enabled:
+            events = self.game_wrapper_pokemon_pinball.handle_events(events)
         # foreach end
         if self.generic_game_wrapper_enabled:
             events = self.generic_game_wrapper.handle_events(events)
         return events
 
     def post_tick(self):
         # foreach plugins [].post_tick()
@@ -153,14 +160,16 @@
             self.game_wrapper_super_mario_land.post_tick()
         if self.game_wrapper_tetris_enabled:
             self.game_wrapper_tetris.post_tick()
         if self.game_wrapper_kirby_dream_land_enabled:
             self.game_wrapper_kirby_dream_land.post_tick()
         if self.game_wrapper_pokemon_gen1_enabled:
             self.game_wrapper_pokemon_gen1.post_tick()
+        if self.game_wrapper_pokemon_pinball_enabled:
+            self.game_wrapper_pokemon_pinball.post_tick()
         # foreach end
         if self.generic_game_wrapper_enabled:
             self.generic_game_wrapper.post_tick()
 
         self._post_tick_windows()
 
     def _set_title(self):
@@ -238,14 +247,16 @@
             title += self.game_wrapper_super_mario_land.window_title()
         if self.game_wrapper_tetris_enabled:
             title += self.game_wrapper_tetris.window_title()
         if self.game_wrapper_kirby_dream_land_enabled:
             title += self.game_wrapper_kirby_dream_land.window_title()
         if self.game_wrapper_pokemon_gen1_enabled:
             title += self.game_wrapper_pokemon_gen1.window_title()
+        if self.game_wrapper_pokemon_pinball_enabled:
+            title += self.game_wrapper_pokemon_pinball.window_title()
         # foreach end
         return title
 
     def stop(self):
         # foreach windows [].stop()
         if self.window_sdl2_enabled:
             self.window_sdl2.stop()
@@ -275,14 +286,16 @@
             self.game_wrapper_super_mario_land.stop()
         if self.game_wrapper_tetris_enabled:
             self.game_wrapper_tetris.stop()
         if self.game_wrapper_kirby_dream_land_enabled:
             self.game_wrapper_kirby_dream_land.stop()
         if self.game_wrapper_pokemon_gen1_enabled:
             self.game_wrapper_pokemon_gen1.stop()
+        if self.game_wrapper_pokemon_pinball_enabled:
+            self.game_wrapper_pokemon_pinball.stop()
         # foreach end
         if self.generic_game_wrapper_enabled:
             self.generic_game_wrapper.stop()
 
     def handle_breakpoint(self):
         if self.debug_prompt_enabled:
             self.debug_prompt.handle_breakpoint()
```

### Comparing `pyboy-2.0.3/pyboy/plugins/manager_gen.py` & `pyboy-2.1.0/pyboy/plugins/manager_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 #
 import re
 
 # Plugins and priority!
 # E.g. DisableInput first
 windows = ["WindowSDL2", "WindowOpenGL", "WindowNull", "Debug"]
 game_wrappers = [
-    "GameWrapperSuperMarioLand", "GameWrapperTetris", "GameWrapperKirbyDreamLand", "GameWrapperPokemonGen1"
+    "GameWrapperSuperMarioLand", "GameWrapperTetris", "GameWrapperKirbyDreamLand", "GameWrapperPokemonGen1",
+    "GameWrapperPokemonPinball"
 ]
 plugins = [
     "DisableInput", "AutoPause", "RecordReplay", "Rewind", "ScreenRecorder", "ScreenshotRecorder", "DebugPrompt"
 ] + game_wrappers
 all_plugins = windows + plugins
```

### Comparing `pyboy-2.0.3/pyboy/plugins/record_replay.py` & `pyboy-2.1.0/pyboy/plugins/record_replay.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/rewind.pxd` & `pyboy-2.1.0/pyboy/plugins/rewind.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/rewind.py` & `pyboy-2.1.0/pyboy/plugins/rewind.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/screen_recorder.py` & `pyboy-2.1.0/pyboy/plugins/screen_recorder.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/screenshot_recorder.py` & `pyboy-2.1.0/pyboy/plugins/screenshot_recorder.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/window_null.py` & `pyboy-2.1.0/pyboy/plugins/window_null.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/window_open_gl.pxd` & `pyboy-2.1.0/pyboy/plugins/window_open_gl.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/window_open_gl.py` & `pyboy-2.1.0/pyboy/plugins/window_open_gl.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/window_sdl2.pxd` & `pyboy-2.1.0/pyboy/plugins/window_sdl2.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/plugins/window_sdl2.py` & `pyboy-2.1.0/pyboy/plugins/window_sdl2.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/pyboy.pxd` & `pyboy-2.1.0/pyboy/pyboy.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/pyboy.py` & `pyboy-2.1.0/pyboy/pyboy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import time
 
 import numpy as np
 
 from pyboy.api.memory_scanner import MemoryScanner
 from pyboy.api.screen import Screen
 from pyboy.api.tilemap import TileMap
-from pyboy.logging import get_logger, log_level
+from pyboy.logging import get_logger
+from pyboy.logging import log_level as _log_level
 from pyboy.plugins.manager import PluginManager, parser_arguments
 from pyboy.utils import IntIOWrapper, WindowEvent
 
 from .api import Sprite, Tile, constants
 from .core.mb import Motherboard
 
 logger = get_logger(__name__)
@@ -45,14 +46,15 @@
         window=defaults["window"],
         scale=defaults["scale"],
         symbols=None,
         bootrom=None,
         sound=False,
         sound_emulated=False,
         cgb=None,
+        log_level=defaults["log_level"],
         **kwargs
     ):
         """
         PyBoy is loadable as an object in Python. This means, it can be initialized from another script, and be
         controlled and probed by the script. It is supported to spawn multiple emulators, just instantiate the class
         multiple times.
 
@@ -79,14 +81,15 @@
             * window (str): "SDL2", "OpenGL", or "null"
             * scale (int): Window scale factor. Doesn't apply to API.
             * symbols (str): Filepath to a .sym file to use. If unsure, specify `None`.
             * bootrom (str): Filepath to a boot-ROM to use. If unsure, specify `None`.
             * sound (bool): Enable sound emulation and output.
             * sound_emulated (bool): Enable sound emulation without any output. Used for compatibility.
             * cgb (bool): Forcing Game Boy Color mode.
+            * log_level (str): "CRITICAL", "ERROR", "WARNING", "INFO" or "DEBUG"
             * color_palette (tuple): Specify the color palette to use for rendering.
             * cgb_color_palette (list of tuple): Specify the color palette to use for rendering in CGB-mode for non-color games.
 
         Other keyword arguments may exist for plugins that are not listed here. They can be viewed by running `pyboy --help` in the terminal.
         """
 
         self.initialized = False
@@ -110,15 +113,18 @@
         kwargs["scale"] = scale
         randomize = kwargs.pop("randomize", False) # Undocumented feature
 
         for k, v in defaults.items():
             if k not in kwargs:
                 kwargs[k] = kwargs.get(k, defaults[k])
 
-        log_level(kwargs.pop("log_level"))
+        _log_level(log_level)
+
+        if gamerom is None:
+            raise FileNotFoundError(f"None is not a ROM file!")
 
         if not os.path.isfile(gamerom):
             raise FileNotFoundError(f"ROM file {gamerom} was not found!")
         self.gamerom = gamerom
 
         self.rom_symbols = {}
         self.rom_symbols_inverse = {}
@@ -1076,14 +1082,20 @@
         >>> pyboy.hook_register(None, "Main.move", lambda x: print(x), "Hello from hook2")
         >>> pyboy.tick(80)
         Hello from hook2
         True
 
         ```
 
+        **NOTE**:
+
+        Don't register hooks to something that isn't executable (graphics data etc.). This will cause your game to show
+        weird behavior or crash. Hooks are installed by replacing the instruction at the bank and address with a special
+        opcode (`0xDB`). If the address is read by the game instead of executed as code, this value will be read instead.
+
         Args:
             bank (int or None): ROM or RAM bank (None for symbol lookup)
             addr (int or str): Address in the Game Boy's address space (str for symbol lookup)
             callback (func): A function which takes `context` as argument
             context (object): Argument to pass to callback when hook is called
         """
         if bank is None and isinstance(addr, str):
@@ -1229,14 +1241,41 @@
         Returns
         -------
         `pyboy.api.tile.Tile`:
             A Tile object for the given identifier.
         """
         return Tile(self.mb, identifier=identifier)
 
+    def rtc_lock_experimental(self, enable):
+        """
+        **WARN: This is an experimental API and is subject to change.**
+
+        Lock the Real Time Clock (RTC) of a supporting cartridge. It might be advantageous to lock the RTC when training
+        an AI in games that use it to change behavior (i.e. day and night).
+
+        The first time the game is turned on, an `.rtc` file is created with the current time. This is the epoch for the
+        RTC. When using `rtc_lock_experimental`, the RTC will always report this point in time. If you let the game progress first,
+        before using `rtc_lock_experimental`, the internal clock will move backwards and might corrupt the game.
+
+        Example:
+        ```python
+        >>> pyboy = PyBoy('game_rom.gb')
+        >>> pyboy.rtc_lock_experimental(True) # RTC will not progress
+        ```
+
+        **WARN: This is an experimental API and is subject to change.**
+
+        Args:
+            enable (float): Point in time to lock RTC to
+        """
+        if self.mb.cartridge.rtc_enabled:
+            self.mb.cartridge.rtc.timelock = enable
+        else:
+            raise Exception("There's no RTC for this cartridge type")
+
 
 class PyBoyMemoryView:
     """
     This class cannot be used directly, but is accessed through `PyBoy.memory`.
 
     This class serves four purposes: Reading memory (ROM/RAM), writing memory (ROM/RAM), overriding memory (ROM/RAM) and special registers.
```

### Comparing `pyboy-2.0.3/pyboy/utils.pxd` & `pyboy-2.1.0/pyboy/utils.pxd`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy/utils.py` & `pyboy-2.1.0/pyboy/utils.py`

 * *Files identical despite different names*

### Comparing `pyboy-2.0.3/pyboy.egg-info/PKG-INFO` & `pyboy-2.1.0/pyboy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboy
-Version: 2.0.3
+Version: 2.1.0
 Summary: Game Boy emulator written in Python
 Author-email: Mads Ynddal <mads@ynddal.dk>
 License: GNU Lesser General Public License
         =================================
         
         _Version 3, 29 June 2007_
         _Copyright © 2007 Free Software Foundation, Inc. &lt;<http://fsf.org/>&gt;_
@@ -249,22 +249,14 @@
 ===============
 The instructions are simple:
 
 ```sh
 $ pip install pyboy
 ```
 
-> [!WARNING]
-> **If you're having issues on Windows, try this instead:** `pip install pyboy==2.0.0 pillow`
->
-> PyPI (who maintains `pip install`) has stopped processing support tickets, and we've been unable to deploy
-> a fix for over a month now. Follow this thread for status: https://github.com/pypi/support/issues/3757
->
-> If you're able to get in contact with PyPI, then please help us get this resolved!
-
 For details, see [installation instructions](https://github.com/Baekalfen/PyBoy/wiki/Installation).
 
 Now you're ready! Either use PyBoy directly from the terminal
 ```sh
 $ pyboy game_rom.gb
 ```
```

### Comparing `pyboy-2.0.3/pyboy.egg-info/SOURCES.txt` & `pyboy-2.1.0/pyboy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 pyboy/plugins/disable_input.pxd
 pyboy/plugins/disable_input.py
 pyboy/plugins/font.txt
 pyboy/plugins/game_wrapper_kirby_dream_land.pxd
 pyboy/plugins/game_wrapper_kirby_dream_land.py
 pyboy/plugins/game_wrapper_pokemon_gen1.pxd
 pyboy/plugins/game_wrapper_pokemon_gen1.py
+pyboy/plugins/game_wrapper_pokemon_pinball.pxd
+pyboy/plugins/game_wrapper_pokemon_pinball.py
 pyboy/plugins/game_wrapper_super_mario_land.pxd
 pyboy/plugins/game_wrapper_super_mario_land.py
 pyboy/plugins/game_wrapper_tetris.pxd
 pyboy/plugins/game_wrapper_tetris.py
 pyboy/plugins/manager.pxd
 pyboy/plugins/manager.py
 pyboy/plugins/manager_gen.py
```

### Comparing `pyboy-2.0.3/pyproject.toml` & `pyboy-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyboy"
-version = "2.0.3"
+version = "2.1.0"
 authors = [
     {name = "Mads Ynddal", email = "mads@ynddal.dk"}
 ]
 keywords = ["gameboy", "game boy", "emulator", "cython", "pypy"]
 description = "Game Boy emulator written in Python"
 readme = "README.md"
 license = {file = "LICENSE.md"}
```

### Comparing `pyboy-2.0.3/setup.py` & `pyboy-2.1.0/setup.py`

 * *Files identical despite different names*

