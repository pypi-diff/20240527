# Comparing `tmp/janim-1.0.4.tar.gz` & `tmp/janim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.0.4.tar` & `janim-1.1.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
--rw-r--r--   0        0        0      165 2024-05-15 13:12:47.689581 janim-1.0.4/.gitignore
--rw-r--r--   0        0        0     1053 2024-05-15 13:12:47.693570 janim-1.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1085 2023-08-02 08:54:33.983910 janim-1.0.4/LICENSE
--rw-r--r--   0        0        0      966 2024-05-15 13:12:47.702546 janim-1.0.4/README.md
--rw-r--r--   0        0        0       71 2024-05-22 00:25:29.846729 janim-1.0.4/janim/__init__.py
--rw-r--r--   0        0        0     3147 2024-05-15 13:12:48.880157 janim-1.0.4/janim/__main__.py
--rw-r--r--   0        0        0     4233 2024-05-15 13:12:48.880157 janim-1.0.4/janim/anims/animation.py
--rw-r--r--   0        0        0     6347 2024-05-20 08:38:15.611875 janim-1.0.4/janim/anims/composition.py
--rw-r--r--   0        0        0     6034 2024-05-15 13:12:48.882153 janim-1.0.4/janim/anims/creation.py
--rw-r--r--   0        0        0      815 2024-05-15 13:12:48.882153 janim-1.0.4/janim/anims/display.py
--rw-r--r--   0        0        0     3454 2024-05-15 13:12:48.883149 janim-1.0.4/janim/anims/fading.py
--rw-r--r--   0        0        0     3954 2024-05-15 13:12:48.884148 janim-1.0.4/janim/anims/growing.py
--rw-r--r--   0        0        0    10342 2024-05-15 13:12:48.884148 janim-1.0.4/janim/anims/indication.py
--rw-r--r--   0        0        0     1547 2024-05-15 13:12:48.885147 janim-1.0.4/janim/anims/rotation.py
--rw-r--r--   0        0        0    26783 2024-05-20 08:38:15.615866 janim-1.0.4/janim/anims/timeline.py
--rw-r--r--   0        0        0     9210 2024-05-15 13:12:48.887139 janim-1.0.4/janim/anims/transform.py
--rw-r--r--   0        0        0     9946 2024-05-19 14:26:49.275303 janim-1.0.4/janim/anims/updater.py
--rw-r--r--   0        0        0     4505 2024-05-15 13:12:48.896116 janim-1.0.4/janim/camera/camera.py
--rw-r--r--   0        0        0     2744 2024-05-15 13:12:48.903096 janim-1.0.4/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6808 2024-05-15 13:12:48.913071 janim-1.0.4/janim/cli.py
--rw-r--r--   0        0        0     9221 2024-05-15 13:12:48.913071 janim-1.0.4/janim/components/component.py
--rw-r--r--   0        0        0     2408 2024-05-15 13:12:48.919053 janim-1.0.4/janim/components/data.py
--rw-r--r--   0        0        0     2609 2024-05-15 13:12:48.919053 janim-1.0.4/janim/components/depth.py
--rw-r--r--   0        0        0     1284 2024-05-15 13:12:48.926037 janim-1.0.4/janim/components/image.py
--rw-r--r--   0        0        0    31079 2024-05-20 08:38:15.620882 janim-1.0.4/janim/components/points.py
--rw-r--r--   0        0        0     2833 2024-05-15 13:12:48.933016 janim-1.0.4/janim/components/radius.py
--rw-r--r--   0        0        0     7927 2024-05-21 15:04:02.417208 janim-1.0.4/janim/components/rgbas.py
--rw-r--r--   0        0        0    22599 2024-05-15 13:12:48.941993 janim-1.0.4/janim/components/vpoints.py
--rw-r--r--   0        0        0      245 2024-05-15 13:12:48.942989 janim-1.0.4/janim/constants/__init__.py
--rw-r--r--   0        0        0      169 2024-05-15 13:12:48.948973 janim-1.0.4/janim/constants/alignment.py
--rw-r--r--   0        0        0     1542 2024-05-15 13:12:48.948973 janim-1.0.4/janim/constants/colors.py
--rw-r--r--   0        0        0      639 2024-05-20 08:38:15.623876 janim-1.0.4/janim/constants/coord.py
--rw-r--r--   0        0        0      179 2024-05-15 13:12:48.961939 janim-1.0.4/janim/constants/degrees.py
--rw-r--r--   0        0        0     4900 2024-05-15 13:12:48.962938 janim-1.0.4/janim/examples.py
--rw-r--r--   0        0        0     1723 2024-05-15 13:12:49.008814 janim-1.0.4/janim/exception.py
--rw-r--r--   0        0        0    41800 2024-05-20 08:38:15.624840 janim-1.0.4/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      330 2024-05-15 13:12:49.015794 janim-1.0.4/janim/gui/application.py
--rw-r--r--   0        0        0      797 2024-05-21 00:09:53.460651 janim-1.0.4/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-05-15 13:12:49.034744 janim-1.0.4/janim/gui/export.png
--rw-r--r--   0        0        0    16958 2024-05-20 08:38:15.625840 janim-1.0.4/janim/gui/favicon.ico
--rw-r--r--   0        0        0     1534 2024-05-20 08:38:15.630824 janim-1.0.4/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0     1465 2024-05-20 08:38:15.634815 janim-1.0.4/janim/gui/glwidget.py
--rw-r--r--   0        0        0      903 2024-05-15 13:12:49.048708 janim-1.0.4/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5278 2024-05-15 13:12:49.058683 janim-1.0.4/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8331 2024-05-15 13:12:49.074245 janim-1.0.4/janim/gui/selector.py
--rw-r--r--   0        0        0     1710 2024-05-20 08:38:15.638834 janim-1.0.4/janim/imports.py
--rw-r--r--   0        0        0     5727 2024-05-15 13:12:49.077235 janim-1.0.4/janim/items/audio.py
--rw-r--r--   0        0        0     5362 2024-05-20 08:38:15.643789 janim-1.0.4/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8745 2024-05-15 13:12:49.078232 janim-1.0.4/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2165 2024-05-15 13:12:49.088209 janim-1.0.4/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8330 2024-05-15 13:12:49.097183 janim-1.0.4/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8784 2024-05-15 13:12:49.108152 janim-1.0.4/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6729 2024-05-15 13:12:49.109152 janim-1.0.4/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7917 2024-05-15 13:12:49.118125 janim-1.0.4/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5239 2024-05-15 13:12:49.119124 janim-1.0.4/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5242 2024-05-20 08:38:15.648777 janim-1.0.4/janim/items/image_item.py
--rw-r--r--   0        0        0    18981 2024-05-21 05:58:39.571823 janim-1.0.4/janim/items/item.py
--rw-r--r--   0        0        0     3262 2024-05-15 13:12:49.122116 janim-1.0.4/janim/items/points.py
--rw-r--r--   0        0        0     7660 2024-05-15 13:12:49.123112 janim-1.0.4/janim/items/relation.py
--rw-r--r--   0        0        0     2071 2024-05-15 13:12:49.131090 janim-1.0.4/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5955 2024-05-15 13:12:49.140067 janim-1.0.4/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1736 2024-05-15 13:12:49.148045 janim-1.0.4/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4432 2024-05-21 15:03:01.842591 janim-1.0.4/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     3090 2024-05-15 13:12:49.158019 janim-1.0.4/janim/items/svg/typst.py
--rw-r--r--   0        0        0       40 2024-05-15 13:12:49.165001 janim-1.0.4/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    16286 2024-05-21 05:45:52.964782 janim-1.0.4/janim/items/text/text.py
--rw-r--r--   0        0        0     1094 2024-05-15 13:12:49.174974 janim-1.0.4/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5357 2024-05-21 05:46:36.179638 janim-1.0.4/janim/items/vitem.py
--rw-r--r--   0        0        0      271 2024-05-15 13:12:49.182953 janim-1.0.4/janim/logger.py
--rw-r--r--   0        0        0     3054 2024-05-15 13:12:49.192927 janim-1.0.4/janim/render/base.py
--rw-r--r--   0        0        0     8857 2024-05-20 08:38:15.653763 janim-1.0.4/janim/render/impl.py
--rw-r--r--   0        0        0      448 2024-05-15 13:12:49.208887 janim-1.0.4/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1250 2024-05-15 13:12:49.216861 janim-1.0.4/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      325 2024-05-15 13:12:49.225837 janim-1.0.4/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      180 2024-05-20 01:53:43.325091 janim-1.0.4/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      350 2024-05-15 13:12:49.247780 janim-1.0.4/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6950 2024-05-15 13:12:49.259747 janim-1.0.4/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      203 2024-05-15 13:12:49.269436 janim-1.0.4/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1091 2024-05-21 13:06:43.084360 janim-1.0.4/janim/render/texture.py
--rw-r--r--   0        0        0     6971 2024-05-20 08:38:15.661774 janim-1.0.4/janim/render/writer.py
--rw-r--r--   0        0        0      964 2024-05-15 13:12:49.278412 janim-1.0.4/janim/typing.py
--rw-r--r--   0        0        0    17207 2024-05-15 13:12:49.289382 janim-1.0.4/janim/utils/bezier.py
--rw-r--r--   0        0        0     5515 2024-05-15 13:12:49.297361 janim-1.0.4/janim/utils/config.py
--rw-r--r--   0        0        0     5786 2024-05-19 13:34:44.597026 janim-1.0.4/janim/utils/data.py
--rw-r--r--   0        0        0      637 2024-05-15 13:12:49.317308 janim-1.0.4/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2483 2024-05-15 13:12:49.330273 janim-1.0.4/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2995 2024-05-15 13:12:49.331270 janim-1.0.4/janim/utils/font.py
--rw-r--r--   0        0        0     6369 2024-05-15 13:12:49.392575 janim-1.0.4/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5973 2024-05-15 13:12:49.403546 janim-1.0.4/janim/utils/iterables.py
--rw-r--r--   0        0        0     1870 2024-05-15 13:12:49.428480 janim-1.0.4/janim/utils/paths.py
--rw-r--r--   0        0        0     2712 2024-05-21 01:50:12.474122 janim-1.0.4/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2651 2024-05-15 13:12:49.435461 janim-1.0.4/janim/utils/refresh.py
--rw-r--r--   0        0        0     8342 2024-05-15 13:12:49.436460 janim-1.0.4/janim/utils/signal.py
--rw-r--r--   0        0        0     2000 2024-05-15 13:12:49.446431 janim-1.0.4/janim/utils/simple_functions.py
--rw-r--r--   0        0        0    10068 2024-05-15 13:12:49.456405 janim-1.0.4/janim/utils/space_ops.py
--rw-r--r--   0        0        0    18504 2024-05-20 08:38:15.667725 janim-1.0.4/logo.png
--rw-r--r--   0        0        0     1030 2024-05-20 08:38:15.671747 janim-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1997 1970-01-01 00:00:00.000000 janim-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      491 2024-05-27 02:44:21.173265 janim-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      153 2024-05-27 02:44:21.173265 janim-1.1.0/.gitignore
+-rw-r--r--   0        0        0       27 2024-05-27 02:44:21.173265 janim-1.1.0/.pypirc
+-rw-r--r--   0        0        0     1011 2024-05-27 02:44:21.173265 janim-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1085 2024-05-27 02:44:21.173265 janim-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1208 2024-05-27 02:44:21.173265 janim-1.1.0/README.md
+-rw-r--r--   0        0        0       68 2024-05-27 02:44:21.217265 janim-1.1.0/janim/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-27 02:44:21.217265 janim-1.1.0/janim/__main__.py
+-rw-r--r--   0        0        0     4108 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/animation.py
+-rw-r--r--   0        0        0     6203 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/composition.py
+-rw-r--r--   0        0        0     5842 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/creation.py
+-rw-r--r--   0        0        0      784 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/display.py
+-rw-r--r--   0        0        0     3329 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/fading.py
+-rw-r--r--   0        0        0     3799 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/growing.py
+-rw-r--r--   0        0        0    12480 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/indication.py
+-rw-r--r--   0        0        0     2375 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/movement.py
+-rw-r--r--   0        0        0     1501 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/rotation.py
+-rw-r--r--   0        0        0    27706 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/timeline.py
+-rw-r--r--   0        0        0     8961 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/transform.py
+-rw-r--r--   0        0        0     9662 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/updater.py
+-rw-r--r--   0        0        0     4360 2024-05-27 02:44:21.217265 janim-1.1.0/janim/camera/camera.py
+-rw-r--r--   0        0        0     2665 2024-05-27 02:44:21.217265 janim-1.1.0/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     6647 2024-05-27 02:44:21.217265 janim-1.1.0/janim/cli.py
+-rw-r--r--   0        0        0     8927 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/component.py
+-rw-r--r--   0        0        0     2331 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/data.py
+-rw-r--r--   0        0        0     2518 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/depth.py
+-rw-r--r--   0        0        0     1239 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/image.py
+-rw-r--r--   0        0        0    30089 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/points.py
+-rw-r--r--   0        0        0     2733 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/radius.py
+-rw-r--r--   0        0        0     7677 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/rgbas.py
+-rw-r--r--   0        0        0    21993 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/vpoints.py
+-rw-r--r--   0        0        0      236 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1469 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/colors.py
+-rw-r--r--   0        0        0      614 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/coord.py
+-rw-r--r--   0        0        0      171 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/degrees.py
+-rw-r--r--   0        0        0     5265 2024-05-27 02:44:21.217265 janim-1.1.0/janim/examples.py
+-rw-r--r--   0        0        0     1654 2024-05-27 02:44:21.217265 janim-1.1.0/janim/exception.py
+-rw-r--r--   0        0        0    41845 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      319 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/application.py
+-rw-r--r--   0        0        0      766 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/export.png
+-rw-r--r--   0        0        0    16958 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/favicon.ico
+-rw-r--r--   0        0        0     1491 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0     1419 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/glwidget.py
+-rw-r--r--   0        0        0      869 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5115 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     8115 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/selector.py
+-rw-r--r--   0        0        0     1699 2024-05-27 02:44:21.221265 janim-1.1.0/janim/imports.py
+-rw-r--r--   0        0        0     7886 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/audio.py
+-rw-r--r--   0        0        0     5190 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8569 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2093 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8078 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8471 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6679 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7653 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5077 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5071 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/image_item.py
+-rw-r--r--   0        0        0    18487 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/item.py
+-rw-r--r--   0        0        0     3150 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/points.py
+-rw-r--r--   0        0        0     7446 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/relation.py
+-rw-r--r--   0        0        0     2012 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5764 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1719 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4298 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     2979 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       37 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    15793 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/text/text.py
+-rw-r--r--   0        0        0     1053 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5204 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/vitem.py
+-rw-r--r--   0        0        0      258 2024-05-27 02:44:21.221265 janim-1.1.0/janim/logger.py
+-rw-r--r--   0        0        0     2951 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/base.py
+-rw-r--r--   0        0        0     8622 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/impl.py
+-rw-r--r--   0        0        0      427 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1200 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      306 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      167 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      332 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6752 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      190 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1069 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/texture.py
+-rw-r--r--   0        0        0     6771 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/writer.py
+-rw-r--r--   0        0        0      931 2024-05-27 02:44:21.221265 janim-1.1.0/janim/typing.py
+-rw-r--r--   0        0        0    16826 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5297 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/config.py
+-rw-r--r--   0        0        0     5590 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/data.py
+-rw-r--r--   0        0        0      618 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2400 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     2896 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/font.py
+-rw-r--r--   0        0        0     6192 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5767 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1810 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/paths.py
+-rw-r--r--   0        0        0     2601 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2566 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8074 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/signal.py
+-rw-r--r--   0        0        0     1919 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0     9707 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    18504 2024-05-27 02:44:21.221265 janim-1.1.0/logo.png
+-rw-r--r--   0        0        0      985 2024-05-27 02:44:21.221265 janim-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 janim-1.1.0/PKG-INFO
```

### Comparing `janim-1.0.4/.readthedocs.yaml` & `janim-1.1.0/.readthedocs.yaml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# .readthedocs.yaml
-# Read the Docs configuration file
-# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
-
-# Required
-version: 2
-
-# Set the OS, Python version and other tools you might need
-build:
-  os: ubuntu-22.04
-  tools:
-    python: "3.12"
-    # You can also specify other tool versions:
-    # nodejs: "19"
-    # rust: "1.64"
-    # golang: "1.19"
-  apt_packages:
-    - portaudio19-dev
-
-# Build documentation in the "docs/" directory with Sphinx
-sphinx:
-  # configuration: docs/conf.py
-  configuration: doc/source/conf.py
-
-# Optionally build your docs in additional formats such as PDF and ePub
-# formats:
-#    - pdf
-#    - epub
-
-# Optional but recommended, declare the Python requirements required
-# to build your documentation
-# See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
-# python:
-#    install:
-#    - requirements: doc/source/requirements.txt
-python:
-  install:
-    - method: pip
-      path: .
-      extra_requirements:
-        - gui
-        - doc
+# .readthedocs.yaml
+# Read the Docs configuration file
+# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
+
+# Required
+version: 2
+
+# Set the OS, Python version and other tools you might need
+build:
+  os: ubuntu-22.04
+  tools:
+    python: "3.12"
+    # You can also specify other tool versions:
+    # nodejs: "19"
+    # rust: "1.64"
+    # golang: "1.19"
+  apt_packages:
+    - portaudio19-dev
+
+# Build documentation in the "docs/" directory with Sphinx
+sphinx:
+  # configuration: docs/conf.py
+  configuration: doc/source/conf.py
+
+# Optionally build your docs in additional formats such as PDF and ePub
+# formats:
+#    - pdf
+#    - epub
+
+# Optional but recommended, declare the Python requirements required
+# to build your documentation
+# See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
+# python:
+#    install:
+#    - requirements: doc/source/requirements.txt
+python:
+  install:
+    - method: pip
+      path: .
+      extra_requirements:
+        - gui
+        - doc
```

### Comparing `janim-1.0.4/LICENSE` & `janim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.0.4/janim/__main__.py` & `janim-1.1.0/janim/__main__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-import os
-from argparse import ArgumentParser, Namespace
-
-from janim.utils.file_ops import get_janim_dir
-
-
-def main() -> None:
-    parser = ArgumentParser(description='A library for simple animation effects')
-    parser.set_defaults(func=None)
-
-    parser.add_argument(
-        '-v', '--version',
-        action='store_true'
-    )
-
-    sp = parser.add_subparsers()
-    run_parser(sp.add_parser('run', help='Run timeline(s) from specific namespace'))
-    write_parser(sp.add_parser('write', help='Generate video file(s) of timeline(s) from specific namesapce'))
-    examples_parser(sp.add_parser('examples', help='Show examples of janim'))
-
-    args = parser.parse_args()
-
-    if args.version:
-        from janim import __version__
-        print(f'JAnim {__version__}')
-
-    if args.func is None:
-        if not args.version:
-            parser.print_help()
-        return
-
-    args.func(args)
-
-
-def render_args(parser: ArgumentParser) -> None:
-    parser.add_argument(
-        'filepath',
-        help='Path to file holding the python code for the timeline'
-    )
-    parser.add_argument(
-        'timeline_names',
-        nargs='*',
-        help='Name of the Timeline class you want to see'
-    )
-    parser.add_argument(
-        '-a', '--all',
-        action='store_true',
-        help='Render all timelines from a file'
-    )
-    parser.add_argument(
-        '-c', '--config',
-        nargs=2,
-        metavar=('key', 'value'),
-        action='append',
-        help='Override config'
-    )
-
-
-def run_parser(parser: ArgumentParser) -> None:
-    render_args(parser)
-    parser.add_argument(
-        '-i', '--interact',
-        action='store_true',
-        help='Enable the network socket for interacting'
-    )
-    parser.set_defaults(func=run)
-
-
-def write_parser(parser: ArgumentParser) -> None:
-    render_args(parser)
-    parser.add_argument(
-        '-o', '--open',
-        action='store_true',
-        help='Open the video after writing'
-    )
-    parser.add_argument(
-        '--format',
-        choices=['mp4', 'mov'],
-        default='mp4',
-        help='Format of the output video'
-    )
-    parser.add_argument(
-        '--audio_format',
-        default='mp3',
-        help='Format of the output audio'
-    )
-    parser.add_argument(
-        '--video',
-        action='store_true',
-    )
-    parser.add_argument(
-        '--audio',
-        action='store_true'
-    )
-    parser.set_defaults(func=write)
-
-
-def examples_parser(parser: ArgumentParser) -> None:
-    parser.set_defaults(filepath=os.path.join(get_janim_dir(), 'examples.py'))
-    parser.add_argument(
-        'timeline_names',
-        nargs='*',
-        help='Name of the example you want to see'
-    )
-    parser.set_defaults(all=None)
-    parser.set_defaults(config=None)
-    parser.set_defaults(func=run)
-    parser.set_defaults(interact=False)
-
-
-def run(args: Namespace) -> None:
-    from janim.cli import run
-    run(args)
-
-
-def write(args: Namespace) -> None:
-    from janim.cli import write
-    write(args)
-
-
-if __name__ == '__main__':
-    main()
+import os
+from argparse import ArgumentParser, Namespace
+
+from janim.utils.file_ops import get_janim_dir
+
+
+def main() -> None:
+    parser = ArgumentParser(description='A library for simple animation effects')
+    parser.set_defaults(func=None)
+
+    parser.add_argument(
+        '-v', '--version',
+        action='store_true'
+    )
+
+    sp = parser.add_subparsers()
+    run_parser(sp.add_parser('run', help='Run timeline(s) from specific namespace'))
+    write_parser(sp.add_parser('write', help='Generate video file(s) of timeline(s) from specific namesapce'))
+    examples_parser(sp.add_parser('examples', help='Show examples of janim'))
+
+    args = parser.parse_args()
+
+    if args.version:
+        from janim import __version__
+        print(f'JAnim {__version__}')
+
+    if args.func is None:
+        if not args.version:
+            parser.print_help()
+        return
+
+    args.func(args)
+
+
+def render_args(parser: ArgumentParser) -> None:
+    parser.add_argument(
+        'filepath',
+        help='Path to file holding the python code for the timeline'
+    )
+    parser.add_argument(
+        'timeline_names',
+        nargs='*',
+        help='Name of the Timeline class you want to see'
+    )
+    parser.add_argument(
+        '-a', '--all',
+        action='store_true',
+        help='Render all timelines from a file'
+    )
+    parser.add_argument(
+        '-c', '--config',
+        nargs=2,
+        metavar=('key', 'value'),
+        action='append',
+        help='Override config'
+    )
+
+
+def run_parser(parser: ArgumentParser) -> None:
+    render_args(parser)
+    parser.add_argument(
+        '-i', '--interact',
+        action='store_true',
+        help='Enable the network socket for interacting'
+    )
+    parser.set_defaults(func=run)
+
+
+def write_parser(parser: ArgumentParser) -> None:
+    render_args(parser)
+    parser.add_argument(
+        '-o', '--open',
+        action='store_true',
+        help='Open the video after writing'
+    )
+    parser.add_argument(
+        '--format',
+        choices=['mp4', 'mov'],
+        default='mp4',
+        help='Format of the output video'
+    )
+    parser.add_argument(
+        '--audio_format',
+        default='mp3',
+        help='Format of the output audio'
+    )
+    parser.add_argument(
+        '--video',
+        action='store_true',
+    )
+    parser.add_argument(
+        '--audio',
+        action='store_true'
+    )
+    parser.set_defaults(func=write)
+
+
+def examples_parser(parser: ArgumentParser) -> None:
+    parser.set_defaults(filepath=os.path.join(get_janim_dir(), 'examples.py'))
+    parser.add_argument(
+        'timeline_names',
+        nargs='*',
+        help='Name of the example you want to see'
+    )
+    parser.set_defaults(all=None)
+    parser.set_defaults(config=None)
+    parser.set_defaults(func=run)
+    parser.set_defaults(interact=False)
+
+
+def run(args: Namespace) -> None:
+    from janim.cli import run
+    run(args)
+
+
+def write(args: Namespace) -> None:
+    from janim.cli import write
+    write(args)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `janim-1.0.4/janim/anims/creation.py` & `janim-1.1.0/janim/anims/creation.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-
-from typing import Callable
-
-import numpy as np
-
-from janim.anims.updater import DataUpdater, UpdaterParams
-from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
-                             C_LABEL_ANIM_OUT, NAN_POINT)
-from janim.items.item import Item
-from janim.items.vitem import VItem
-from janim.typing import JAnimColor
-from janim.utils.bezier import integer_interpolate
-from janim.utils.rate_functions import RateFunc, double_smooth, linear
-
-
-class ShowPartial(DataUpdater):
-    '''
-    显示物件一部分的动画，显示的部分由 ``bound_func`` 决定
-    '''
-    label_color = C_LABEL_ANIM_ABSTRACT
-
-    def __init__(
-        self,
-        item: Item,
-        bound_func: Callable[[UpdaterParams], tuple[int, int]],
-        *,
-        auto_close_path: bool = False,
-        become_at_end: bool = False,
-        root_only: bool = False,
-        **kwargs
-    ):
-        def func(data: Item, p: UpdaterParams) -> None:
-            cmpt = data.components.get('points', None)
-            if cmpt is None or not isinstance(cmpt, Cmpt_VPoints):
-                return  # pragma: no cover
-            if not cmpt.has():
-                return  # pragma: no cover
-
-            if not auto_close_path:
-                cmpt.pointwise_become_partial(cmpt, *bound_func(p))     # pragma: no cover
-            else:
-                end_indices = np.array(cmpt.get_subpath_end_indices())
-                begin_indices = np.array([0, *[indice + 2 for indice in end_indices[:-1]]])
-
-                points = cmpt.get()
-                cond1 = np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
-
-                cmpt.pointwise_become_partial(cmpt, *bound_func(p))
-
-                points = cmpt.get().copy()
-                cond2 = ~np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
-                where = np.where(cond1 & cond2)[0]
-
-                if len(where) == 0:
-                    return
-
-                end_indices = end_indices[where]
-                begin_indices = begin_indices[where]
-
-                points[end_indices] = points[begin_indices]
-                if end_indices[-1] == len(points) - 1:
-                    end_indices = end_indices[:-1]
-                points[end_indices + 1] = NAN_POINT
-
-                cmpt.set(points)
-
-        super().__init__(item, func, become_at_end=become_at_end, root_only=root_only, **kwargs)
-
-
-class Create(ShowPartial):
-    '''
-    显示物件的创建过程
-    '''
-    label_color = C_LABEL_ANIM_IN
-
-    def __init__(self, item: Item, auto_close_path: bool = True, **kwargs):
-        super().__init__(item, lambda p: (0, p.alpha), auto_close_path=auto_close_path, **kwargs)
-
-
-class Uncreate(ShowPartial):
-    '''
-    显示物件的销毁过程（:class:`Create` 的倒放）
-    '''
-    label_color = C_LABEL_ANIM_OUT
-
-    def __init__(
-        self,
-        item: Item,
-        show_at_end: bool = False,
-        auto_close_path: bool = True,
-        **kwargs
-    ):
-        super().__init__(
-            item,
-            lambda p: (0, 1.0 - p.alpha),
-            show_at_end=show_at_end,
-            auto_close_path=auto_close_path,
-            **kwargs
-        )
-
-
-class DrawBorderThenFill(DataUpdater):
-    '''
-    画出边缘，然后填充颜色
-    '''
-    label_color = C_LABEL_ANIM_IN
-
-    def __init__(
-        self,
-        item: Item,
-        *,
-        duration: float = 2.0,
-        stroke_radius: float = 0.01,
-        stroke_color: JAnimColor = None,
-        rate_func: RateFunc = double_smooth,
-        become_at_end: bool = False,
-        root_only: bool = False,
-        **kwargs
-    ):
-        super().__init__(
-            item,
-            self.updater,
-            duration=duration,
-            rate_func=rate_func,
-            become_at_end=become_at_end,
-            root_only=root_only,
-            **kwargs
-        )
-        self.stroke_radius = stroke_radius
-        self.stroke_color = stroke_color
-
-    def create_extra_data(self, data: Item) -> VItem | None:
-        if not isinstance(data, VItem):
-            return None     # pragma: no cover
-        data_copy = data.store()
-        data_copy.radius.set(self.stroke_radius)
-        data_copy.stroke.set(self.stroke_color, 1)
-        data_copy.fill.set(alpha=0)
-        return data_copy
-
-    def updater(self, data: VItem, p: UpdaterParams) -> None:
-        if p.extra_data is None:
-            return  # pragma: no cover
-        outline = p.extra_data
-        index, subalpha = integer_interpolate(0, 2, p.alpha)
-
-        if index == 0:
-            data.restore(outline)
-            data.points.pointwise_become_partial(data.points, 0, subalpha)
-        else:
-            data.interpolate(outline, data, subalpha)
-
-
-class Write(DrawBorderThenFill):
-    '''
-    显示书写过程（对每个子物件应用 :class:`DrawBorderThenFill`）
-    '''
-    def __init__(
-        self,
-        item: Item,
-        *,
-        duration: float | None = None,
-        lag_ratio: float | None = None,
-        rate_func: RateFunc = linear,
-        skip_null_items: bool = True,
-        root_only: bool = False,
-        **kwargs
-    ):
-        length = len([
-            item
-            for item in (
-                [self.item]
-                if root_only
-                else item.walk_self_and_descendants()
-            )
-            if not skip_null_items or not item.is_null()
-        ])
-        if duration is None:
-            duration = 1 if length < 15 else 2
-        if lag_ratio is None:
-            lag_ratio = min(4.0 / (length + 1.0), 0.2)
-
-        super().__init__(
-            item,
-            duration=duration,
-            lag_ratio=lag_ratio,
-            rate_func=rate_func,
-            skip_null_items=skip_null_items,
-            root_only=root_only,
-            **kwargs
-        )
+
+from typing import Callable
+
+import numpy as np
+
+from janim.anims.updater import DataUpdater, UpdaterParams
+from janim.components.vpoints import Cmpt_VPoints
+from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
+                             C_LABEL_ANIM_OUT, NAN_POINT)
+from janim.items.item import Item
+from janim.items.vitem import VItem
+from janim.typing import JAnimColor
+from janim.utils.bezier import integer_interpolate
+from janim.utils.rate_functions import RateFunc, double_smooth, linear
+
+
+class ShowPartial(DataUpdater):
+    '''
+    显示物件一部分的动画，显示的部分由 ``bound_func`` 决定
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
+    def __init__(
+        self,
+        item: Item,
+        bound_func: Callable[[UpdaterParams], tuple[int, int]],
+        *,
+        auto_close_path: bool = False,
+        become_at_end: bool = False,
+        root_only: bool = False,
+        **kwargs
+    ):
+        def func(data: Item, p: UpdaterParams) -> None:
+            cmpt = data.components.get('points', None)
+            if cmpt is None or not isinstance(cmpt, Cmpt_VPoints):
+                return  # pragma: no cover
+            if not cmpt.has():
+                return  # pragma: no cover
+
+            if not auto_close_path:
+                cmpt.pointwise_become_partial(cmpt, *bound_func(p))     # pragma: no cover
+            else:
+                end_indices = np.array(cmpt.get_subpath_end_indices())
+                begin_indices = np.array([0, *[indice + 2 for indice in end_indices[:-1]]])
+
+                points = cmpt.get()
+                cond1 = np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
+
+                cmpt.pointwise_become_partial(cmpt, *bound_func(p))
+
+                points = cmpt.get().copy()
+                cond2 = ~np.isclose(points[begin_indices], points[end_indices]).all(axis=1)
+                where = np.where(cond1 & cond2)[0]
+
+                if len(where) == 0:
+                    return
+
+                end_indices = end_indices[where]
+                begin_indices = begin_indices[where]
+
+                points[end_indices] = points[begin_indices]
+                if end_indices[-1] == len(points) - 1:
+                    end_indices = end_indices[:-1]
+                points[end_indices + 1] = NAN_POINT
+
+                cmpt.set(points)
+
+        super().__init__(item, func, become_at_end=become_at_end, root_only=root_only, **kwargs)
+
+
+class Create(ShowPartial):
+    '''
+    显示物件的创建过程
+    '''
+    label_color = C_LABEL_ANIM_IN
+
+    def __init__(self, item: Item, auto_close_path: bool = True, **kwargs):
+        super().__init__(item, lambda p: (0, p.alpha), auto_close_path=auto_close_path, **kwargs)
+
+
+class Uncreate(ShowPartial):
+    '''
+    显示物件的销毁过程（:class:`Create` 的倒放）
+    '''
+    label_color = C_LABEL_ANIM_OUT
+
+    def __init__(
+        self,
+        item: Item,
+        show_at_end: bool = False,
+        auto_close_path: bool = True,
+        **kwargs
+    ):
+        super().__init__(
+            item,
+            lambda p: (0, 1.0 - p.alpha),
+            show_at_end=show_at_end,
+            auto_close_path=auto_close_path,
+            **kwargs
+        )
+
+
+class DrawBorderThenFill(DataUpdater):
+    '''
+    画出边缘，然后填充颜色
+    '''
+    label_color = C_LABEL_ANIM_IN
+
+    def __init__(
+        self,
+        item: Item,
+        *,
+        duration: float = 2.0,
+        stroke_radius: float = 0.01,
+        stroke_color: JAnimColor = None,
+        rate_func: RateFunc = double_smooth,
+        become_at_end: bool = False,
+        root_only: bool = False,
+        **kwargs
+    ):
+        super().__init__(
+            item,
+            self.updater,
+            duration=duration,
+            rate_func=rate_func,
+            become_at_end=become_at_end,
+            root_only=root_only,
+            **kwargs
+        )
+        self.stroke_radius = stroke_radius
+        self.stroke_color = stroke_color
+
+    def create_extra_data(self, data: Item) -> VItem | None:
+        if not isinstance(data, VItem):
+            return None     # pragma: no cover
+        data_copy = data.store()
+        data_copy.radius.set(self.stroke_radius)
+        data_copy.stroke.set(self.stroke_color, 1)
+        data_copy.fill.set(alpha=0)
+        return data_copy
+
+    def updater(self, data: VItem, p: UpdaterParams) -> None:
+        if p.extra_data is None:
+            return  # pragma: no cover
+        outline = p.extra_data
+        index, subalpha = integer_interpolate(0, 2, p.alpha)
+
+        if index == 0:
+            data.restore(outline)
+            data.points.pointwise_become_partial(data.points, 0, subalpha)
+        else:
+            data.interpolate(outline, data, subalpha)
+
+
+class Write(DrawBorderThenFill):
+    '''
+    显示书写过程（对每个子物件应用 :class:`DrawBorderThenFill`）
+    '''
+    def __init__(
+        self,
+        item: Item,
+        *,
+        duration: float | None = None,
+        lag_ratio: float | None = None,
+        rate_func: RateFunc = linear,
+        skip_null_items: bool = True,
+        root_only: bool = False,
+        **kwargs
+    ):
+        length = len([
+            item
+            for item in (
+                [self.item]
+                if root_only
+                else item.walk_self_and_descendants()
+            )
+            if not skip_null_items or not item.is_null()
+        ])
+        if duration is None:
+            duration = 1 if length < 15 else 2
+        if lag_ratio is None:
+            lag_ratio = min(4.0 / (length + 1.0), 0.2)
+
+        super().__init__(
+            item,
+            duration=duration,
+            lag_ratio=lag_ratio,
+            rate_func=rate_func,
+            skip_null_items=skip_null_items,
+            root_only=root_only,
+            **kwargs
+        )
```

### Comparing `janim-1.0.4/janim/anims/fading.py` & `janim-1.1.0/janim/anims/fading.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-
-from abc import ABCMeta, abstractmethod
-
-import numpy as np
-
-from janim.anims.updater import DataUpdater, UpdaterParams
-from janim.components.rgbas import Cmpt_Rgbas
-from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
-                             C_LABEL_ANIM_OUT, ORIGIN)
-from janim.items.item import Item
-from janim.items.points import Points
-from janim.typing import Vect
-
-
-class Fade(DataUpdater, metaclass=ABCMeta):
-    '''
-    :class:`FadeIn` 和 :class:`FadeOut` 的基类
-    '''
-    label_color = C_LABEL_ANIM_ABSTRACT
-
-    def __init__(
-        self,
-        item: Item,
-        shift: Vect = ORIGIN,
-        scale: float = 1.0,
-        *,
-        about_point: Vect | None = None,
-        about_edge: Vect = ORIGIN,
-        become_at_end: bool = False,
-        root_only: bool = False,
-        **kwargs
-    ):
-        super().__init__(
-            item,
-            self.updater,
-            become_at_end=become_at_end,
-            root_only=root_only,
-            **kwargs
-        )
-        self.shift = shift
-        self.scale = scale
-
-        if about_point is None and scale != 1.0:
-            cmpt = item(Points).points
-            box = cmpt.self_box if root_only else cmpt.box
-            about_point = box.get(about_edge)
-        self.about_point = about_point
-
-    @abstractmethod
-    def updater(self, data: Item, p: UpdaterParams) -> None:
-        pass
-
-
-class FadeIn(Fade):
-    '''
-    淡入
-
-    - 可以使用 ``shift`` 指定淡入位移
-    - 可以使用 ``scale`` 指定淡入缩放
-    '''
-    label_color = C_LABEL_ANIM_IN
-
-    def updater(self, data: Item, p: UpdaterParams) -> None:
-        if not isinstance(data, Points):
-            return
-
-        for cmpt in data.components.values():
-            if not isinstance(cmpt, Cmpt_Rgbas):
-                continue
-            rgbas = cmpt.get().copy()
-            rgbas[:, 3] *= p.alpha
-            cmpt.set_rgbas(rgbas)
-
-        if np.any(self.shift != ORIGIN):
-            data.points.shift((1 - p.alpha) * -self.shift)
-        if self.scale != 1.0:
-            data.points.scale(
-                (1 - p.alpha) * 1 / self.scale + p.alpha,
-                about_point=self.about_point
-            )
-
-
-class FadeOut(Fade):
-    '''
-    淡出
-
-    - 可以使用 ``shift`` 指定淡出位移
-    - 可以使用 ``scale`` 指定淡出缩放
-    '''
-    label_color = C_LABEL_ANIM_OUT
-
-    def __init__(
-        self,
-        item: Item,
-        shift: Vect = ORIGIN,
-        scale: float = 1.0,
-        show_at_end: float = False,
-        **kwargs
-    ):
-        super().__init__(
-            item,
-            shift,
-            scale,
-            show_at_end=show_at_end,
-            **kwargs
-        )
-
-    def updater(self, data: Item, p: UpdaterParams) -> None:
-        if not isinstance(data, Points):
-            return
-
-        for cmpt in data.components.values():
-            if not isinstance(cmpt, Cmpt_Rgbas):
-                continue
-            rgbas = cmpt.get().copy()
-            rgbas[:, 3] *= 1 - p.alpha
-            cmpt.set_rgbas(rgbas)
-
-        if np.any(self.shift != ORIGIN):
-            data.points.shift(p.alpha * self.shift)
-        if self.scale != 1.0:
-            data.points.scale(
-                p.alpha * self.scale + (1 - p.alpha),
-                about_point=self.about_point
-            )
+
+from abc import ABCMeta, abstractmethod
+
+import numpy as np
+
+from janim.anims.updater import DataUpdater, UpdaterParams
+from janim.components.rgbas import Cmpt_Rgbas
+from janim.constants import (C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN,
+                             C_LABEL_ANIM_OUT, ORIGIN)
+from janim.items.item import Item
+from janim.items.points import Points
+from janim.typing import Vect
+
+
+class Fade(DataUpdater, metaclass=ABCMeta):
+    '''
+    :class:`FadeIn` 和 :class:`FadeOut` 的基类
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
+    def __init__(
+        self,
+        item: Item,
+        shift: Vect = ORIGIN,
+        scale: float = 1.0,
+        *,
+        about_point: Vect | None = None,
+        about_edge: Vect = ORIGIN,
+        become_at_end: bool = False,
+        root_only: bool = False,
+        **kwargs
+    ):
+        super().__init__(
+            item,
+            self.updater,
+            become_at_end=become_at_end,
+            root_only=root_only,
+            **kwargs
+        )
+        self.shift = shift
+        self.scale = scale
+
+        if about_point is None and scale != 1.0:
+            cmpt = item(Points).points
+            box = cmpt.self_box if root_only else cmpt.box
+            about_point = box.get(about_edge)
+        self.about_point = about_point
+
+    @abstractmethod
+    def updater(self, data: Item, p: UpdaterParams) -> None:
+        pass
+
+
+class FadeIn(Fade):
+    '''
+    淡入
+
+    - 可以使用 ``shift`` 指定淡入位移
+    - 可以使用 ``scale`` 指定淡入缩放
+    '''
+    label_color = C_LABEL_ANIM_IN
+
+    def updater(self, data: Item, p: UpdaterParams) -> None:
+        if not isinstance(data, Points):
+            return
+
+        for cmpt in data.components.values():
+            if not isinstance(cmpt, Cmpt_Rgbas):
+                continue
+            rgbas = cmpt.get().copy()
+            rgbas[:, 3] *= p.alpha
+            cmpt.set_rgbas(rgbas)
+
+        if np.any(self.shift != ORIGIN):
+            data.points.shift((1 - p.alpha) * -self.shift)
+        if self.scale != 1.0:
+            data.points.scale(
+                (1 - p.alpha) * 1 / self.scale + p.alpha,
+                about_point=self.about_point
+            )
+
+
+class FadeOut(Fade):
+    '''
+    淡出
+
+    - 可以使用 ``shift`` 指定淡出位移
+    - 可以使用 ``scale`` 指定淡出缩放
+    '''
+    label_color = C_LABEL_ANIM_OUT
+
+    def __init__(
+        self,
+        item: Item,
+        shift: Vect = ORIGIN,
+        scale: float = 1.0,
+        show_at_end: float = False,
+        **kwargs
+    ):
+        super().__init__(
+            item,
+            shift,
+            scale,
+            show_at_end=show_at_end,
+            **kwargs
+        )
+
+    def updater(self, data: Item, p: UpdaterParams) -> None:
+        if not isinstance(data, Points):
+            return
+
+        for cmpt in data.components.values():
+            if not isinstance(cmpt, Cmpt_Rgbas):
+                continue
+            rgbas = cmpt.get().copy()
+            rgbas[:, 3] *= 1 - p.alpha
+            cmpt.set_rgbas(rgbas)
+
+        if np.any(self.shift != ORIGIN):
+            data.points.shift(p.alpha * self.shift)
+        if self.scale != 1.0:
+            data.points.scale(
+                p.alpha * self.scale + (1 - p.alpha),
+                about_point=self.about_point
+            )
```

### Comparing `janim-1.0.4/janim/anims/growing.py` & `janim-1.1.0/janim/anims/growing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from __future__ import annotations
-
-from typing import Callable
-
-import numpy as np
-
-from janim.anims.animation import Animation, RenderCall
-from janim.anims.transform import Transform
-from janim.constants import C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN, PI
-from janim.items.geometry.arrow import Arrow
-from janim.items.points import Points
-
-
-class GrowFromPoint(Transform):
-    '''
-    从指定的位置放大显现
-    '''
-    label_color = C_LABEL_ANIM_IN
-
-    def __init__(
-        self,
-        item: Points,
-        point: np.ndarray,
-        *,
-        hide_src: bool = True,
-        **kwargs
-    ):
-        self.point = point
-        self.start_item = item.copy()
-        self.start_item.points.scale(0).move_to(point)
-        super().__init__(self.start_item, item, hide_src=hide_src, **kwargs)
-
-    def anim_init(self) -> None:
-        super().anim_init()
-        if self.hide_src:
-            self.timeline.schedule(self.global_range.at, self.target_item.hide, root_only=self.root_only)
-
-
-class GrowFromCenter(GrowFromPoint):
-    '''从物件的中心放大显现'''
-    def __init__(self, item: Points, **kwargs):
-        point = item.points.box.center
-        super().__init__(item, point, **kwargs)
-
-
-class GrowFromEdge(GrowFromPoint):
-    '''从物件的指定边角放大显现'''
-    def __init__(self, item: Points, edge: np.ndarray, **kwargs):
-        point = item.points.box.get(edge)
-        super().__init__(item, point, **kwargs)
-
-
-class GrowArrowByBoundFunc(Animation):
-    '''显示箭头的显现过程，从开头到结尾画出，并自动调整箭头标志位置'''
-    label_color = C_LABEL_ANIM_ABSTRACT
-
-    def __init__(
-        self,
-        arrow: Arrow,
-        bound_func: Callable[[float], tuple[float, float]],
-        *,
-        hide_at_begin: bool = True,
-        show_at_end: bool = True,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.arrow = arrow
-        self.bound_func = bound_func
-        self.hide_at_begin = hide_at_begin
-        self.show_at_end = show_at_end
-
-        self.timeline.track(arrow)
-
-    def anim_init(self) -> None:
-        self.arrow_copy = self.arrow.copy()
-        self.arrow_anim = self.arrow.copy()
-
-        self.set_render_call_list([
-            RenderCall(
-                item.depth,
-                item.render
-            )
-            for item in self.arrow_anim.walk_self_and_descendants()
-        ])
-
-        if self.hide_at_begin:
-            self.timeline.schedule(self.global_range.at, self.arrow.hide)
-        if self.show_at_end:
-            self.timeline.schedule(self.global_range.end, self.arrow.show)
-
-    def anim_on_alpha(self, alpha: float) -> None:
-        self.arrow_anim.points.pointwise_become_partial(self.arrow_copy, *self.bound_func(alpha))
-        self.arrow_anim.place_tip()
-
-
-class GrowArrow(GrowArrowByBoundFunc):
-    '''显示箭头的显现过程，从开头到结尾画出，并自动调整箭头标志位置'''
-    label_color = C_LABEL_ANIM_IN
-
-    def __init__(self, arrow: Arrow, **kwargs):
-        super().__init__(arrow, lambda alpha: (0, alpha), **kwargs)
-
-
-class GrowDoubleArrow(GrowArrowByBoundFunc):
-    '''
-    显示箭头的显现过程，默认从中间向两边显现，并自动调整箭头标志位置
-
-    - 传入 ``start_ratio``（默认 ``0.5``） 可以调整开始的位置
-    '''
-    label_color = C_LABEL_ANIM_IN
-
-    def __init__(self, arrow: Arrow, start_ratio: float = 0.5, **kwargs):
-        super().__init__(
-            arrow,
-            lambda alpha: (start_ratio * (1 - alpha), 1 - (1 - start_ratio) * (1 - alpha)),
-            **kwargs
-        )
-
-
-class SpinInFromNothing(GrowFromCenter):
-    '''从物件的中心旋转半圈放大显现'''
-    def __init__(self, item: Points, *, path_arc=PI, **kwargs):
-        super().__init__(item, path_arc=path_arc, **kwargs)
+from __future__ import annotations
+
+from typing import Callable
+
+import numpy as np
+
+from janim.anims.animation import Animation, RenderCall
+from janim.anims.transform import Transform
+from janim.constants import C_LABEL_ANIM_ABSTRACT, C_LABEL_ANIM_IN, PI
+from janim.items.geometry.arrow import Arrow
+from janim.items.points import Points
+
+
+class GrowFromPoint(Transform):
+    '''
+    从指定的位置放大显现
+    '''
+    label_color = C_LABEL_ANIM_IN
+
+    def __init__(
+        self,
+        item: Points,
+        point: np.ndarray,
+        *,
+        hide_src: bool = True,
+        **kwargs
+    ):
+        self.point = point
+        self.start_item = item.copy()
+        self.start_item.points.scale(0).move_to(point)
+        super().__init__(self.start_item, item, hide_src=hide_src, **kwargs)
+
+    def anim_init(self) -> None:
+        super().anim_init()
+        if self.hide_src:
+            self.timeline.schedule(self.global_range.at, self.target_item.hide, root_only=self.root_only)
+
+
+class GrowFromCenter(GrowFromPoint):
+    '''从物件的中心放大显现'''
+    def __init__(self, item: Points, **kwargs):
+        point = item.points.box.center
+        super().__init__(item, point, **kwargs)
+
+
+class GrowFromEdge(GrowFromPoint):
+    '''从物件的指定边角放大显现'''
+    def __init__(self, item: Points, edge: np.ndarray, **kwargs):
+        point = item.points.box.get(edge)
+        super().__init__(item, point, **kwargs)
+
+
+class SpinInFromNothing(GrowFromCenter):
+    '''从物件的中心旋转半圈放大显现'''
+    def __init__(self, item: Points, *, path_arc=PI, **kwargs):
+        super().__init__(item, path_arc=path_arc, **kwargs)
+
+
+class GrowArrowByBoundFunc(Animation):
+    ''':class:`GrowArrow` 和 :class:`GrowDoubleArrow` 的基类'''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
+    def __init__(
+        self,
+        arrow: Arrow,
+        bound_func: Callable[[float], tuple[float, float]],
+        *,
+        hide_at_begin: bool = True,
+        show_at_end: bool = True,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        self.arrow = arrow
+        self.bound_func = bound_func
+        self.hide_at_begin = hide_at_begin
+        self.show_at_end = show_at_end
+
+        self.timeline.track(arrow)
+
+    def anim_init(self) -> None:
+        self.arrow_copy = self.arrow.copy()
+        self.arrow_anim = self.arrow.copy()
+
+        self.set_render_call_list([
+            RenderCall(
+                item.depth,
+                item.render
+            )
+            for item in self.arrow_anim.walk_self_and_descendants()
+        ])
+
+        if self.hide_at_begin:
+            self.timeline.schedule(self.global_range.at, self.arrow.hide)
+        if self.show_at_end:
+            self.timeline.schedule(self.global_range.end, self.arrow.show)
+
+    def anim_on_alpha(self, alpha: float) -> None:
+        self.arrow_anim.points.pointwise_become_partial(self.arrow_copy, *self.bound_func(alpha))
+        self.arrow_anim.place_tip()
+
+
+class GrowArrow(GrowArrowByBoundFunc):
+    '''显示箭头的显现过程，从开头到结尾画出，并自动调整箭头标志位置'''
+    label_color = C_LABEL_ANIM_IN
+
+    def __init__(self, arrow: Arrow, **kwargs):
+        super().__init__(arrow, lambda alpha: (0, alpha), **kwargs)
+
+
+class GrowDoubleArrow(GrowArrowByBoundFunc):
+    '''
+    显示箭头的显现过程，默认从中间向两边显现，并自动调整箭头标志位置
+
+    - 传入 ``start_ratio`` （默认 ``0.5``） 可以调整开始的位置
+    '''
+    label_color = C_LABEL_ANIM_IN
+
+    def __init__(self, arrow: Arrow, start_ratio: float = 0.5, **kwargs):
+        super().__init__(
+            arrow,
+            lambda alpha: (start_ratio * (1 - alpha), 1 - (1 - start_ratio) * (1 - alpha)),
+            **kwargs
+        )
```

### Comparing `janim-1.0.4/janim/anims/timeline.py` & `janim-1.1.0/janim/anims/timeline.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,772 +1,826 @@
-from __future__ import annotations
-
-import heapq
-import inspect
-import math
-import time
-import traceback
-from abc import ABCMeta, abstractmethod
-from bisect import bisect, insort
-from collections import defaultdict
-from contextvars import ContextVar
-from dataclasses import dataclass
-from typing import Callable, Iterable, Self, overload
-
-import moderngl as mgl
-import numpy as np
-from PIL import Image
-
-from janim.anims.animation import Animation, TimeRange
-from janim.anims.composition import AnimGroup
-from janim.anims.display import Display
-from janim.anims.updater import updater_params_ctx
-from janim.camera.camera import Camera
-from janim.constants import BLACK, DEFAULT_DURATION, DOWN, SMALL_BUFF, UP
-from janim.exception import TimelineLookupError
-from janim.items.audio import Audio
-from janim.items.item import DynamicItem, Item
-from janim.items.points import Group
-from janim.items.shape_matchers import SurroundingRect
-from janim.items.svg.typst import TypstText
-from janim.items.text.text import Text
-from janim.logger import log
-from janim.render.base import RenderData, Renderer, set_global_uniforms
-from janim.typing import JAnimColor
-from janim.utils.config import Config, ConfigGetter, config_ctx_var
-from janim.utils.data import ContextSetter, History
-from janim.utils.iterables import resize_preserving_order
-from janim.utils.simple_functions import clip
-
-
-class Timeline(metaclass=ABCMeta):
-    '''
-    继承该类并实现 :meth:`construct` 方法，以实现动画的构建逻辑
-
-    调用 :meth:`build` 可以得到构建完成的动画对象
-    '''
-
-    # region config
-
-    CONFIG: Config | None = None
-    '''
-    在子类中定义该变量可以起到设置配置的作用，例如：
-
-    .. code-block::
-
-        class Example(Timeline):
-            CONFIG = Config(
-                font=['Consolas', 'LXGW WenKai Lite']
-            )
-
-            def construct(self) -> None:
-                ...
-
-    另见：:class:`~.Config`
-    '''
-
-    class _WithConfig:
-        def __init__(self, cls: type[Timeline]):
-            self.cls = cls
-
-            self.lst: list[Config] = []
-            for sup in self.cls.mro():
-                config: Config | None = getattr(sup, 'CONFIG', None)
-                if config is None or config in self.lst:
-                    continue
-                self.lst.append(config)
-
-            self.lst.reverse()
-
-        def __enter__(self) -> Self:
-            lst = [*config_ctx_var.get(), *self.lst]
-            self.token = config_ctx_var.set(lst)
-            return self
-
-        def __exit__(self, exc_type, exc_value, tb) -> None:
-            config_ctx_var.reset(self.token)
-
-    @classmethod
-    def with_config(cls) -> _WithConfig:
-        '''
-        使用定义在 :class:`Timeline` 子类中的 config
-        '''
-        return cls._WithConfig(cls)
-
-    # endregion
-
-    # region context
-
-    ctx_var: ContextVar[Timeline | None] = ContextVar('Timeline.ctx_var', default=None)
-
-    @staticmethod
-    def get_context(raise_exc=True) -> Timeline | None:
-        '''
-        调用该方法可以得到当前正在构建的 :class:`Timeline` 对象
-
-        - 如果在 :meth:`construct` 方法外调用，且 ``raise_exc=True`` （默认），则抛出 :class:`~.TimelineLookupError`
-        '''
-        obj = Timeline.ctx_var.get(None)
-        if obj is None and raise_exc:
-            f_back = inspect.currentframe().f_back
-            raise TimelineLookupError(f'{f_back.f_code.co_qualname} 无法在 Timeline.construct 之外使用')
-        return obj
-
-    # endregion
-
-    @dataclass
-    class TimeOfCode:
-        '''
-        标记 :meth:`~.Timeline.construct` 执行到的代码行数所对应的时间
-        '''
-        time: float
-        line: int
-
-    @dataclass
-    class ScheduledTask:
-        '''
-        另见 :meth:`~.Timeline.schedule`
-        '''
-        at: float
-        func: Callable
-        args: list
-        kwargs: dict
-
-    @dataclass
-    class PlayAudioInfo:
-        '''
-        调用 :meth:`~.Timeline.play_audio` 的参数信息
-        '''
-        audio: Audio
-        range: TimeRange
-        clip_range: TimeRange
-
-    @dataclass
-    class SubtitleInfo:
-        '''
-        调用 :meth:`~.Timeline.subtitle` 的参数信息
-        '''
-        text: str
-        range: TimeRange
-        kwargs: dict
-        subtitle: Text
-
-    class ItemHistory:
-        def __init__(self):
-            self.history: History[Item | DynamicItem] = History()
-            self.history_without_dynamic: History[Item] = History()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self.current_time: float = 0
-        self.times_of_code: list[Timeline.TimeOfCode] = []
-
-        self.scheduled_tasks: list[Timeline.ScheduledTask] = []
-        self.anims: list[AnimGroup] = []
-        self.display_anims: list[Display] = []
-        self.audio_infos: list[Timeline.PlayAudioInfo] = []
-        self.subtitle_infos: list[Timeline.SubtitleInfo] = []   # helpful for extracting subtitles
-
-        self.items_history: defaultdict[Item, Timeline.ItemHistory] = defaultdict(Timeline.ItemHistory)
-        self.item_display_times: dict[Item, int] = {}
-
-    @abstractmethod
-    def construct(self) -> None:
-        '''
-        继承该方法以实现动画的构建逻辑
-        '''
-        pass    # pragma: no cover
-
-    def build(self, *, quiet=False) -> TimelineAnim:
-        '''
-        构建动画并返回
-        '''
-        with self.with_config(), ContextSetter(self.ctx_var, self):
-
-            self.config_getter = ConfigGetter(config_ctx_var.get())
-            self.camera = Camera()
-
-            self._build_frame = inspect.currentframe()
-
-            if not quiet:   # pragma: no cover
-                log.info(f'Building "{self.__class__.__name__}"')
-                start_time = time.time()
-
-            self.construct()
-
-            if self.current_time == 0:
-                self.forward(DEFAULT_DURATION)  # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
-                if not quiet:   # pragma: no cover
-                    log.info(f'"{self.__class__.__name__}" 构建后没有产生时长，自动产生了 {DEFAULT_DURATION}s 的时长')
-            self.cleanup_display()
-            global_anim = TimelineAnim(self)
-
-            if not quiet:   # pragma: no cover
-                elapsed = time.time() - start_time
-                log.info(f'Finished building "{self.__class__.__name__}" in {elapsed:.2f} s')
-
-        return global_anim
-
-    def schedule(self, at: float, func: Callable, *args, **kwargs) -> None:
-        '''
-        计划执行
-
-        会在进度达到 ``at`` 时，对 ``func`` 进行调用，
-        可传入 ``*args`` 和 ``**kwargs``
-        '''
-        rough_at = round(at, 4)   # 防止因为精度误差使得本来计划更迟的任务被更早地执行了
-        task = Timeline.ScheduledTask(rough_at, func, args, kwargs)
-        insort(self.scheduled_tasks, task, key=lambda x: x.at)
-        task.at = at
-
-    # region progress
-
-    def forward(self, dt: float = 1, *, _detect_changes=True) -> None:
-        '''
-        向前推进 ``dt`` 秒
-        '''
-        if dt <= 0:
-            raise ValueError('dt 必须大于 0')
-
-        if _detect_changes:
-            self.detect_changes_of_all()
-
-        to_time = self.current_time + dt
-
-        while self.scheduled_tasks and self.scheduled_tasks[0].at <= to_time:
-            task = self.scheduled_tasks.pop(0)
-            self.current_time = task.at
-            task.func(*task.args, **task.kwargs)
-
-        self.current_time = to_time
-
-        self.times_of_code.append(
-            Timeline.TimeOfCode(
-                self.current_time,
-                self.get_construct_lineno() or -1
-            )
-        )
-
-    def forward_to(self, t: float, *, _detect_changes=True) -> None:
-        '''
-        向前推进到 ``t`` 秒的时候
-        '''
-        self.forward(t - self.current_time, _detect_changes=_detect_changes)
-
-    def prepare(self, *anims: Animation, **kwargs) -> TimeRange:
-        '''
-        应用动画
-        '''
-        anim = AnimGroup(*anims, **kwargs)
-        anim.local_range.at += self.current_time
-        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
-
-        anim.anim_pre_init()
-        self.detect_changes_of_all()
-        anim.anim_init()
-
-        self.anims.append(anim)
-
-        return anim.local_range
-
-    def play(self, *anims: Animation, **kwargs) -> None:
-        '''
-        应用动画并推进到动画结束的时候
-        '''
-        t_range = self.prepare(*anims, **kwargs)
-        self.forward_to(t_range.end, _detect_changes=False)
-
-    # endregion
-
-    # region display
-
-    def is_displaying(self, item: Item) -> None:
-        '''
-        判断特定的物件是否正在显示中
-
-        另见：:meth:`show`、:meth:`hide`
-        '''
-        return item in self.item_display_times
-
-    def _show(self, item: Item) -> None:
-        self.item_display_times.setdefault(item, self.current_time)
-
-    def show(self, *roots: Item, root_only=False) -> None:
-        '''
-        显示物件
-        '''
-        for root in roots:
-            self._show(root)
-            if not root_only:
-                for item in root.descendants():
-                    self._show(item)
-
-    def _hide(self, item: Item) -> Display:
-        time = self.item_display_times.pop(item, None)
-        if time is None:
-            return
-
-        duration = self.current_time - time
-
-        anim = Display(item, duration=duration)
-        anim.local_range.at += time
-        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
-        self.display_anims.append(anim)
-        return anim
-
-    def hide(self, *roots: Item, root_only=False) -> None:
-        '''
-        隐藏物件
-        '''
-        for root in roots:
-            self._hide(root)
-            if not root_only:
-                for item in root.descendants():
-                    self._hide(item)
-
-    def cleanup_display(self) -> None:
-        '''
-        对目前显示中的所有物件调用隐藏，使得正确产生 :class:`~.Display` 对象
-        '''
-        for item in list(self.item_display_times.keys()):
-            self._hide(item)
-
-    # endregion
-
-    # region audio
-
-    def play_audio(
-        self,
-        audio: Audio,
-        *,
-        delay: float = 0,
-        begin: float = 0,
-        end: float = -1,
-    ) -> TimeRange:
-        '''
-        在当前位置播放音频
-
-        - 可以指定 ``begin`` 和 ``end`` 表示裁剪区段
-        - 可以指定在当前位置往后 ``delay`` 秒才开始播放
-
-        返回值表示播放的时间段
-        '''
-        if end == -1:
-            end = audio.duration()
-        duration = end - begin
-
-        info = Timeline.PlayAudioInfo(audio,
-                                      TimeRange(self.current_time + delay, duration),
-                                      TimeRange(begin, duration))
-        self.audio_infos.append(info)
-
-        return info.range.copy()
-
-    def has_audio(self) -> bool:
-        '''
-        是否有可以播放的音频
-        '''
-        return len(self.audio_infos) != 0
-
-    def get_audio_samples_of_frame(
-        self,
-        fps: float,
-        framerate: int,
-        frame: int
-    ) -> np.ndarray:
-        '''
-        提取特定帧的音频流
-        '''
-        begin = frame / fps
-        end = (frame + 1) / fps
-
-        output_sample_count = math.floor(end * framerate) - math.floor(begin * framerate)
-        result = np.zeros(output_sample_count, dtype=np.int16)
-
-        for info in self.audio_infos:
-            if end < info.range.at or begin > info.range.end:
-                continue
-
-            audio = info.audio
-
-            frame_begin = int((begin - info.range.at + info.clip_range.at) * audio.framerate)
-            frame_end = int((end - info.range.at + info.clip_range.at) * audio.framerate)
-
-            clip_begin = max(0, int(audio.framerate * info.clip_range.at))
-            clip_end = min(audio.sample_count(), int(audio.framerate * info.clip_range.end))
-
-            left_blank = max(0, clip_begin - frame_begin)
-            right_blank = max(0, frame_end - clip_end)
-
-            data = audio._samples.data[max(clip_begin, frame_begin): min(clip_end, frame_end)]
-
-            if left_blank != 0 or right_blank != 0:
-                data = np.concatenate([
-                    np.zeros(left_blank, dtype=np.int16),
-                    data,
-                    np.zeros(right_blank, dtype=np.int16)
-                ])
-
-            result += resize_preserving_order(data, output_sample_count)
-
-        return result
-
-    # endregion
-
-    # region subtitle
-
-    @overload
-    def subtitle(
-        self,
-        text: str | Iterable[str],
-        duration: float = 1,
-        delay: float = 0,
-        scale: float | Iterable[float] = 0.8,
-        use_typst_text: bool | Iterable[bool] = False,
-        **kwargs
-    ) -> TimeRange: ...
-
-    @overload
-    def subtitle(self, text: str | Iterable[str], range: TimeRange, **kwargs) -> TimeRange: ...
-
-    def subtitle(
-        self,
-        text: str | Iterable[str],
-        duration: float = 1,
-        delay: float = 0,
-        scale: float | Iterable[float] = 1,
-        base_scale: float = 0.8,
-        use_typst_text: bool | Iterable[bool] = False,
-        surrounding_color: JAnimColor = BLACK,
-        surrounding_alpha: float = 0.5,
-        **kwargs
-    ) -> TimeRange:
-        '''
-        添加字幕
-
-        - 文字可以传入一个列表，纵向排列显示
-        - 可以指定在当前位置往后 ``delay`` 秒才显示
-        - ``duration`` 表示持续时间
-        - ``scale`` 表示对文字的缩放，默认为 ``0.8``，可以传入列表表示对各个文字的缩放
-        - ``use_typst_text`` 表示是否使用 :class:`TypstText`，可以传入列表表示各个文字是否使用
-
-        返回值表示显示的时间段
-        '''
-        text_lst = [text] if isinstance(text, str) else text
-        scale_lst = [scale] if not isinstance(scale, Iterable) else scale
-        use_typst_lst = [use_typst_text] if not isinstance(use_typst_text, Iterable) else use_typst_text
-
-        if isinstance(duration, TimeRange):
-            range = duration
-        else:
-            range = TimeRange(self.current_time + delay, duration)
-
-        for text, scale, use_typst_text in zip(reversed(text_lst),
-                                               reversed(resize_preserving_order(scale_lst, len(text_lst))),
-                                               reversed(resize_preserving_order(use_typst_lst, len(text_lst)))):
-            subtitle = (TypstText if use_typst_text else Text)(text, **kwargs)
-            subtitle.depth.set(-1e5)
-            subtitle.points.scale(scale * base_scale)
-            self.place_subtitle(subtitle, range)
-            self.subtitle_infos.append(Timeline.SubtitleInfo(text,
-                                                             range,
-                                                             kwargs,
-                                                             subtitle))
-
-            subtitle_group = Group(
-                SurroundingRect(subtitle,
-                                color=surrounding_color,
-                                stroke_alpha=0,
-                                fill_alpha=surrounding_alpha),
-                subtitle
-            )
-            subtitle_group.depth.arrange(subtitle.depth.get())
-
-            self.schedule(range.at, subtitle_group.show)
-            self.schedule(range.end, subtitle_group.hide)
-
-        return range.copy()
-
-    def place_subtitle(self, subtitle: Text, range: TimeRange) -> None:
-        '''
-        被 :meth:`subtitle` 调用以将字幕放置到合适的位置：
-
-        - 对于同一批添加的字幕 ``[a, b]``，则 ``a`` 放在 ``b`` 的上面
-        - 如果在上文所述的 ``[a, b]`` 仍存在时，又加入了一个 ``c``，则 ``c`` 放在最上面
-        '''
-        for other in reversed(self.subtitle_infos):
-            # 根据 TimelineView 中排列显示标签的经验
-            # 这里加了一个 np.isclose 的判断
-            # 如果不加可能导致前一个字幕消失但是后一个字幕凭空出现在更上面
-            # （但是我没有测试过是否会出现这个bug，只是根据写 TimelineView 时的经验加了 np.isclose）
-            if other.range.at <= range.at < other.range.end and not np.isclose(range.at, other.range.end):
-                subtitle.points.next_to(other.subtitle, UP, buff=SMALL_BUFF)
-                return
-        subtitle.points.to_border(DOWN)
-
-    # endregion
-
-    # region history
-
-    def track(self, item: Item) -> None:
-        '''
-        使得 ``item`` 在每次 ``forward`` 和 ``play`` 时都会被自动调用 :meth:`~.Item.detect_change`
-        '''
-        self.items_history[item]
-
-    def detect_changes_of_all(self) -> None:
-        '''
-        检查所有物件是否有产生变化并记录
-        '''
-        for item, ih in self.items_history.items():
-            self._detect_change(item, ih, as_time=self.current_time)
-
-    def detect_changes(self, items: Iterable[Item], *, as_time: float | None = None) -> None:
-        '''
-        检查指定的列表中的物件是否有产生变化并记录（仅检查自身而不包括子物件的）
-        '''
-        if as_time is None:
-            as_time = self.current_time
-        for item in items:
-            self._detect_change(item, self.items_history[item], as_time=as_time)
-
-    @staticmethod
-    def _detect_change(item: Item, ih: ItemHistory, *, as_time: float) -> None:
-        history_wo_dnmc = ih.history_without_dynamic
-        if not history_wo_dnmc.has_record() or not history_wo_dnmc.latest().data.not_changed(item):
-            item_copy = item.store()
-            ih.history.record_as_time(as_time, item_copy)
-            history_wo_dnmc.record_as_time(as_time, item_copy)
-
-    def register_dynamic(
-        self,
-        item: Item,
-        dynamic: DynamicItem,
-        static: Item | None,
-        begin: float,
-        end: float,
-        static_replaceable: bool
-    ) -> None:
-        ih = self.items_history[item]
-        ih.history.record_as_time(begin, dynamic)
-
-        if static is None:
-            if ih.history_without_dynamic.has_record():
-                static = ih.history_without_dynamic.latest().data
-            else:
-                static = item.store()
-        ih.history.record_as_time(end, static, replaceable=static_replaceable)
-        ih.history_without_dynamic.record_as_time(end, static, replaceable=static_replaceable)
-
-    def item_current[T](self, item: T, *, as_time: float | None = None, skip_dynamic=False) -> T:
-        '''
-        另见 :meth:`~.Item.current`
-        '''
-        ih = self.items_history[item]
-        history = ih.history_without_dynamic if skip_dynamic else ih.history
-        if not history.has_record():
-            return item
-
-        if as_time is None:
-            params = updater_params_ctx.get(None)
-            if params is not None:
-                as_time = params.global_t
-        if as_time is None:
-            as_time = Animation.global_t_ctx.get(None)
-
-        if as_time is None:
-            return item
-
-        item_or_dynamic = history.get(as_time)
-        return item_or_dynamic if isinstance(item_or_dynamic, Item) else item_or_dynamic(as_time)
-
-    # endregion
-
-    # region lineno
-
-    def get_construct_lineno(self) -> int | None:
-        '''
-        得到当前在 :meth:`construct` 中执行到的行数
-        '''
-        frame = inspect.currentframe().f_back
-        while frame is not None:
-            f_back = frame.f_back
-
-            if f_back is self._build_frame:
-                return frame.f_lineno
-
-            frame = f_back
-
-        return None     # pragma: no cover
-
-    def get_lineno_at_time(self, time: float):
-        '''
-        根据 ``time`` 得到对应执行到的行数
-        '''
-        times_of_code = self.times_of_code
-        if not times_of_code:
-            return -1
-
-        idx = bisect(times_of_code, time, key=lambda x: x.time)
-        idx = clip(idx, 0, len(times_of_code) - 1)
-        return times_of_code[idx].line
-
-    # endregion
-
-    # region debug
-
-    @staticmethod
-    def fmt_time(t: float) -> str:
-        time = round(t, 3)
-
-        minutes = int(time // 60)
-        time %= 60
-
-        hours = minutes // 60
-        minutes %= 60
-
-        seconds = math.floor(time)
-        ms = round((time - seconds) * 1e3)
-
-        times = []
-        if hours != 0:
-            times.append(f'{hours}h')
-        times.append(f'{minutes:>3d}m' if minutes != 0 else ' ' * 4)
-        times.append(f'{seconds:>3d}s')
-        times.append(f'{ms:>4d}ms' if ms != 0 else ' ' * 6)
-
-        return "".join(times)
-
-    def dbg_time(self, ext_msg: str = '') -> None:  # pragma: no cover
-        if ext_msg:
-            ext_msg = f'[{ext_msg}]  '
-
-        time = self.fmt_time(self.current_time)
-
-        log.debug(f't={time}  {ext_msg}at construct.{self.get_construct_lineno()}')
-
-    # endregion
-
-
-class SourceTimeline(Timeline):     # pragma: no cover
-    '''
-    与 :class:`Timeline` 相比，会在背景显示源代码
-    '''
-    def build(self, *, quiet=False) -> TimelineAnim:
-        from janim.items.text.text import SourceDisplayer
-        with ContextSetter(self.ctx_var, self):
-            SourceDisplayer(self.__class__).show()
-        return super().build(quiet=quiet)
-
-
-class TimelineAnim(AnimGroup):
-    '''
-    运行 :meth:`Timeline.run` 后返回的动画组
-
-    - ``self.display_anim`` 是由 :meth:`Timeline.construct` 中执行
-      :meth:`Timeline.show` 和 :meth:`Timeline.hide` 而产生的
-    - ``self.user_anim`` 是显式使用了 :meth:`Timeline.prepare` 或 :meth:`Timeline.play` 而产生的
-    '''
-    def __init__(self, timeline: Timeline, **kwargs):
-        self.timeline = timeline
-
-        self.display_anim = AnimGroup(*timeline.display_anims)
-        self.user_anim = AnimGroup(*timeline.anims)
-        super().__init__(self.display_anim, self.user_anim, **kwargs)
-        self.maxt = self.local_range.duration = timeline.current_time
-
-        self.display_anim.global_range = self.display_anim.local_range
-        self.user_anim.global_range = self.user_anim.local_range
-        self.global_range = self.local_range
-
-        self.flattened = self.flatten()
-        self._time: float | None = None
-
-    @property
-    def cfg(self) -> Config | ConfigGetter:
-        return self.timeline.config_getter
-
-    def anim_on(self, local_t: float) -> None:
-        # 使最后一帧不空屏
-        if np.isclose(local_t, self.global_range.duration):
-            local_t -= 1 / self.cfg.fps
-
-        self._time = local_t
-        with ContextSetter(self.global_t_ctx, local_t):
-            super().anim_on(local_t)
-
-    def render_all(self, ctx: mgl.Context) -> None:
-        '''
-        调用所有的 :class:`RenderCall` 进行渲染
-        '''
-        if self._time is None:
-            return
-
-        try:
-            with ContextSetter(Animation.global_t_ctx, self._time):
-                timeline = self.timeline
-                camera_info = timeline.camera.current().points.info
-                anti_alias_radius = self.cfg.anti_alias_width / 2 * camera_info.scaled_factor
-
-                set_global_uniforms(
-                    ctx,
-                    ('JA_VIEW_MATRIX', camera_info.view_matrix.T.flatten()),
-                    ('JA_PROJ_MATRIX', camera_info.proj_matrix.T.flatten()),
-                    ('JA_FRAME_RADIUS', camera_info.frame_radius),
-                    ('JA_ANTI_ALIAS_RADIUS', anti_alias_radius)
-                )
-
-                with ContextSetter(Renderer.data_ctx, RenderData(ctx=ctx,
-                                                                 camera_info=camera_info,
-                                                                 anti_alias_radius=anti_alias_radius)):
-                    # 使用 heapq 以深度为序调用 RenderCall
-                    render_calls = heapq.merge(
-                        *[
-                            anim.render_call_list
-                            for anim in self.flattened
-                            if anim.render_call_list and anim.global_range.at <= self._time < anim.global_range.end
-                        ],
-                        key=lambda x: x.depth,
-                        reverse=True
-                    )
-                    for render_call in render_calls:
-                        render_call.func()
-
-        except Exception:
-            traceback.print_exc()
-
-    capture_ctx: mgl.Context | None = None
-    capture_fbo: mgl.Framebuffer | None = None
-
-    def capture(self) -> Image.Image:
-        if TimelineAnim.capture_ctx is None:
-            TimelineAnim.capture_ctx = mgl.create_standalone_context(require=430)
-            TimelineAnim.capture_ctx.enable(mgl.BLEND)
-            TimelineAnim.capture_ctx.blend_func = (
-                mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
-                mgl.ONE, mgl.ONE
-            )
-            TimelineAnim.capture_ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
-
-            pw, ph = self.cfg.pixel_width, self.cfg.pixel_height
-            TimelineAnim.capture_fbo = TimelineAnim.capture_ctx.framebuffer(
-                color_attachments=TimelineAnim.capture_ctx.texture(
-                    (pw, ph),
-                    components=4,
-                    samples=0,
-                ),
-                depth_attachment=TimelineAnim.capture_ctx.depth_renderbuffer(
-                    (pw, ph),
-                    samples=0
-                )
-            )
-
-        fbo = TimelineAnim.capture_fbo
-        fbo.use()
-        fbo.clear(*self.cfg.background_color.rgb)
-        self.render_all(TimelineAnim.capture_ctx)
-
-        return Image.frombytes(
-            "RGBA", fbo.size, fbo.read(components=4),
-            "raw", "RGBA", 0, -1
-        )
+from __future__ import annotations
+
+import heapq
+import inspect
+import math
+import time
+import traceback
+import types
+from abc import ABCMeta, abstractmethod
+from bisect import bisect, insort
+from collections import defaultdict
+from contextvars import ContextVar
+from dataclasses import dataclass
+from typing import Callable, Iterable, Self, overload
+
+import moderngl as mgl
+import numpy as np
+from PIL import Image
+
+from janim.anims.animation import Animation, TimeRange
+from janim.anims.composition import AnimGroup
+from janim.anims.display import Display
+from janim.anims.updater import updater_params_ctx
+from janim.camera.camera import Camera
+from janim.constants import BLACK, DEFAULT_DURATION, DOWN, SMALL_BUFF, UP
+from janim.exception import TimelineLookupError
+from janim.items.audio import Audio
+from janim.items.item import DynamicItem, Item
+from janim.items.points import Group
+from janim.items.shape_matchers import SurroundingRect
+from janim.items.svg.typst import TypstText
+from janim.items.text.text import Text
+from janim.logger import log
+from janim.render.base import RenderData, Renderer, set_global_uniforms
+from janim.typing import JAnimColor
+from janim.utils.config import Config, ConfigGetter, config_ctx_var
+from janim.utils.data import ContextSetter, History
+from janim.utils.iterables import resize_preserving_order
+from janim.utils.simple_functions import clip
+
+
+class Timeline(metaclass=ABCMeta):
+    '''
+    继承该类并实现 :meth:`construct` 方法，以实现动画的构建逻辑
+
+    调用 :meth:`build` 可以得到构建完成的动画对象
+    '''
+
+    # region config
+
+    CONFIG: Config | None = None
+    '''
+    在子类中定义该变量可以起到设置配置的作用，例如：
+
+    .. code-block::
+
+        class Example(Timeline):
+            CONFIG = Config(
+                font=['Consolas', 'LXGW WenKai Lite']
+            )
+
+            def construct(self) -> None:
+                ...
+
+    另见：:class:`~.Config`
+    '''
+
+    class _WithConfig:
+        def __init__(self, cls: type[Timeline]):
+            self.cls = cls
+
+            self.lst: list[Config] = []
+            for sup in self.cls.mro():
+                config: Config | None = getattr(sup, 'CONFIG', None)
+                if config is None or config in self.lst:
+                    continue
+                self.lst.append(config)
+
+            self.lst.reverse()
+
+        def __enter__(self) -> Self:
+            lst = [*config_ctx_var.get(), *self.lst]
+            self.token = config_ctx_var.set(lst)
+            return self
+
+        def __exit__(self, exc_type, exc_value, tb) -> None:
+            config_ctx_var.reset(self.token)
+
+    @classmethod
+    def with_config(cls) -> _WithConfig:
+        '''
+        使用定义在 :class:`Timeline` 子类中的 config
+        '''
+        return cls._WithConfig(cls)
+
+    # endregion
+
+    # region context
+
+    ctx_var: ContextVar[Timeline | None] = ContextVar('Timeline.ctx_var', default=None)
+
+    @staticmethod
+    def get_context(raise_exc=True) -> Timeline | None:
+        '''
+        调用该方法可以得到当前正在构建的 :class:`Timeline` 对象
+
+        - 如果在 :meth:`construct` 方法外调用，且 ``raise_exc=True`` （默认），则抛出 :class:`~.TimelineLookupError`
+        '''
+        obj = Timeline.ctx_var.get(None)
+        if obj is None and raise_exc:
+            f_back = inspect.currentframe().f_back
+            raise TimelineLookupError(f'{f_back.f_code.co_qualname} 无法在 Timeline.construct 之外使用')
+        return obj
+
+    # endregion
+
+    @dataclass
+    class TimeOfCode:
+        '''
+        标记 :meth:`~.Timeline.construct` 执行到的代码行数所对应的时间
+        '''
+        time: float
+        line: int
+
+    @dataclass
+    class ScheduledTask:
+        '''
+        另见 :meth:`~.Timeline.schedule`
+        '''
+        at: float
+        func: Callable
+        args: list
+        kwargs: dict
+
+    @dataclass
+    class PlayAudioInfo:
+        '''
+        调用 :meth:`~.Timeline.play_audio` 的参数信息
+        '''
+        audio: Audio
+        range: TimeRange
+        clip_range: TimeRange
+
+    @dataclass
+    class SubtitleInfo:
+        '''
+        调用 :meth:`~.Timeline.subtitle` 的参数信息
+        '''
+        text: str
+        range: TimeRange
+        kwargs: dict
+        subtitle: Text
+
+    class ItemHistory:
+        def __init__(self):
+            self.history: History[Item | DynamicItem] = History()
+            self.history_without_dynamic: History[Item] = History()
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.current_time: float = 0
+        self.times_of_code: list[Timeline.TimeOfCode] = []
+
+        self.scheduled_tasks: list[Timeline.ScheduledTask] = []
+        self.anims: list[AnimGroup] = []
+        self.display_anims: list[Display] = []
+        self.audio_infos: list[Timeline.PlayAudioInfo] = []
+        self.subtitle_infos: list[Timeline.SubtitleInfo] = []   # helpful for extracting subtitles
+
+        self.items_history: defaultdict[Item, Timeline.ItemHistory] = defaultdict(Timeline.ItemHistory)
+        self.item_display_times: dict[Item, int] = {}
+
+    @abstractmethod
+    def construct(self) -> None:
+        '''
+        继承该方法以实现动画的构建逻辑
+        '''
+        pass    # pragma: no cover
+
+    def build(self, *, quiet=False) -> TimelineAnim:
+        '''
+        构建动画并返回
+        '''
+        with self.with_config(), ContextSetter(self.ctx_var, self):
+
+            self.config_getter = ConfigGetter(config_ctx_var.get())
+            self.camera = Camera()
+
+            self._build_frame = inspect.currentframe()
+
+            if not quiet:   # pragma: no cover
+                log.info(f'Building "{self.__class__.__name__}"')
+                start_time = time.time()
+
+            self.construct()
+
+            if self.current_time == 0:
+                self.forward(DEFAULT_DURATION)  # 使得没有任何前进时，产生一点时间，避免除零以及其它问题
+                if not quiet:   # pragma: no cover
+                    log.info(f'"{self.__class__.__name__}" 构建后没有产生时长，自动产生了 {DEFAULT_DURATION}s 的时长')
+            self.cleanup_display()
+            global_anim = TimelineAnim(self)
+
+            if not quiet:   # pragma: no cover
+                elapsed = time.time() - start_time
+                log.info(f'Finished building "{self.__class__.__name__}" in {elapsed:.2f} s')
+
+        return global_anim
+
+    def schedule(self, at: float, func: Callable, *args, **kwargs) -> None:
+        '''
+        计划执行
+
+        会在进度达到 ``at`` 时，对 ``func`` 进行调用，
+        可传入 ``*args`` 和 ``**kwargs``
+        '''
+        rough_at = round(at, 4)   # 防止因为精度误差使得本来计划更迟的任务被更早地执行了
+        task = Timeline.ScheduledTask(rough_at, func, args, kwargs)
+        insort(self.scheduled_tasks, task, key=lambda x: x.at)
+        task.at = at
+
+    # region progress
+
+    def forward(self, dt: float = 1, *, _detect_changes=True) -> None:
+        '''
+        向前推进 ``dt`` 秒
+        '''
+        if dt <= 0:
+            raise ValueError('dt 必须大于 0')
+
+        if _detect_changes:
+            self.detect_changes_of_all()
+
+        to_time = self.current_time + dt
+
+        while self.scheduled_tasks and self.scheduled_tasks[0].at <= to_time:
+            task = self.scheduled_tasks.pop(0)
+            self.current_time = task.at
+            task.func(*task.args, **task.kwargs)
+
+        self.current_time = to_time
+
+        self.times_of_code.append(
+            Timeline.TimeOfCode(
+                self.current_time,
+                self.get_construct_lineno() or -1
+            )
+        )
+
+    def forward_to(self, t: float, *, _detect_changes=True) -> None:
+        '''
+        向前推进到 ``t`` 秒的时候
+        '''
+        self.forward(t - self.current_time, _detect_changes=_detect_changes)
+
+    def prepare(self, *anims: Animation, **kwargs) -> TimeRange:
+        '''
+        应用动画
+        '''
+        anim = AnimGroup(*anims, **kwargs)
+        anim.local_range.at += self.current_time
+        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
+
+        anim.anim_pre_init()
+        self.detect_changes_of_all()
+        anim.anim_init()
+
+        self.anims.append(anim)
+
+        return anim.local_range
+
+    def play(self, *anims: Animation, **kwargs) -> None:
+        '''
+        应用动画并推进到动画结束的时候
+        '''
+        t_range = self.prepare(*anims, **kwargs)
+        self.forward_to(t_range.end, _detect_changes=False)
+
+    # endregion
+
+    # region display
+
+    def is_displaying(self, item: Item) -> None:
+        '''
+        判断特定的物件是否正在显示中
+
+        另见：:meth:`show`、:meth:`hide`
+        '''
+        return item in self.item_display_times
+
+    def _show(self, item: Item) -> None:
+        self.item_display_times.setdefault(item, self.current_time)
+
+    def show(self, *roots: Item, root_only=False) -> None:
+        '''
+        显示物件
+        '''
+        for root in roots:
+            self._show(root)
+            if not root_only:
+                for item in root.descendants():
+                    self._show(item)
+
+    def _hide(self, item: Item) -> Display:
+        time = self.item_display_times.pop(item, None)
+        if time is None:
+            return
+
+        duration = self.current_time - time
+
+        anim = Display(item, duration=duration)
+        anim.local_range.at += time
+        anim.compute_global_range(anim.local_range.at, anim.local_range.duration)
+        self.display_anims.append(anim)
+        return anim
+
+    def hide(self, *roots: Item, root_only=False) -> None:
+        '''
+        隐藏物件
+        '''
+        for root in roots:
+            self._hide(root)
+            if not root_only:
+                for item in root.descendants():
+                    self._hide(item)
+
+    def cleanup_display(self) -> None:
+        '''
+        对目前显示中的所有物件调用隐藏，使得正确产生 :class:`~.Display` 对象
+        '''
+        for item in list(self.item_display_times.keys()):
+            self._hide(item)
+
+    # endregion
+
+    # region audio_and_subtitle
+
+    def aas(
+        self,
+        file_path: str,
+        subtitle: str | Iterable[str],
+        **kwargs
+    ) -> TimeRange:
+        '''
+        :meth:`audio_and_subtitle` 的简写
+        '''
+        return self.audio_and_subtitle(file_path, subtitle, **kwargs)
+
+    def audio_and_subtitle(
+        self,
+        file_path: str,
+        subtitle: str | Iterable[str],
+        *,
+        clip: tuple[float, float] | None | types.EllipsisType = ...,
+        delay: float = 0,
+        mul: float | Iterable[float] | None = None,
+        **subtitle_kwargs
+    ) -> TimeRange:
+        '''
+        播放音频，并在对应的区间显示字幕
+
+        - 如果 ``clip=...`` （默认，省略号），则表示自动确定裁剪区间，将前后的空白去除（可以传入 ``clip=None`` 禁用自动裁剪）
+        - 如果 ``mul`` 不是 ``None``，则会将音频振幅乘以该值
+        '''
+        audio = Audio(file_path)
+        if mul is not None:
+            audio.mul(mul)
+
+        if clip is ...:
+            recommended = audio.recommended_range()
+            if recommended is None:
+                clip = None
+            else:
+                clip = (math.floor(recommended[0] * 10) / 10,
+                        math.ceil(recommended[1] * 10) / 10)
+
+        t = self.play_audio(audio, delay=delay, clip=clip)
+        self.subtitle(subtitle, t, **subtitle_kwargs)
+
+        return t
+
+    # region audio
+
+    def play_audio(
+        self,
+        audio: Audio,
+        *,
+        delay: float = 0,
+        begin: float = 0,
+        end: float = -1,
+        clip: tuple[float, float] | None = None,
+    ) -> TimeRange:
+        '''
+        在当前位置播放音频
+
+        - 可以指定 ``begin`` 和 ``end`` 表示裁剪区段
+        - 可以指定在当前位置往后 ``delay`` 秒才开始播放
+        - 若指定 ``clip``，则会覆盖 ``begin`` 和 ``end`` （可以将 ``clip`` 视为这二者的简写）
+
+        返回值表示播放的时间段
+        '''
+        if clip is not None:
+            begin, end = clip
+
+        if end == -1:
+            end = audio.duration()
+        duration = end - begin
+
+        info = Timeline.PlayAudioInfo(audio,
+                                      TimeRange(self.current_time + delay, duration),
+                                      TimeRange(begin, duration))
+        self.audio_infos.append(info)
+
+        return info.range.copy()
+
+    def has_audio(self) -> bool:
+        '''
+        是否有可以播放的音频
+        '''
+        return len(self.audio_infos) != 0
+
+    def get_audio_samples_of_frame(
+        self,
+        fps: float,
+        framerate: int,
+        frame: int
+    ) -> np.ndarray:
+        '''
+        提取特定帧的音频流
+        '''
+        begin = frame / fps
+        end = (frame + 1) / fps
+
+        output_sample_count = math.floor(end * framerate) - math.floor(begin * framerate)
+        result = np.zeros(output_sample_count, dtype=np.int16)
+
+        for info in self.audio_infos:
+            if end < info.range.at or begin > info.range.end:
+                continue
+
+            audio = info.audio
+
+            frame_begin = int((begin - info.range.at + info.clip_range.at) * audio.framerate)
+            frame_end = int((end - info.range.at + info.clip_range.at) * audio.framerate)
+
+            clip_begin = max(0, int(audio.framerate * info.clip_range.at))
+            clip_end = min(audio.sample_count(), int(audio.framerate * info.clip_range.end))
+
+            left_blank = max(0, clip_begin - frame_begin)
+            right_blank = max(0, frame_end - clip_end)
+
+            data = audio._samples.data[max(clip_begin, frame_begin): min(clip_end, frame_end)]
+
+            if left_blank != 0 or right_blank != 0:
+                data = np.concatenate([
+                    np.zeros(left_blank, dtype=np.int16),
+                    data,
+                    np.zeros(right_blank, dtype=np.int16)
+                ])
+
+            result += resize_preserving_order(data, output_sample_count)
+
+        return result
+
+    # endregion
+
+    # region subtitle
+
+    @overload
+    def subtitle(
+        self,
+        text: str | Iterable[str],
+        duration: float = 1,
+        delay: float = 0,
+        scale: float | Iterable[float] = 0.8,
+        use_typst_text: bool | Iterable[bool] = False,
+        **kwargs
+    ) -> TimeRange: ...
+
+    @overload
+    def subtitle(self, text: str | Iterable[str], range: TimeRange, **kwargs) -> TimeRange: ...
+
+    def subtitle(
+        self,
+        text: str | Iterable[str],
+        duration: float = 1,
+        delay: float = 0,
+        scale: float | Iterable[float] = 1,
+        base_scale: float = 0.8,
+        use_typst_text: bool | Iterable[bool] = False,
+        surrounding_color: JAnimColor = BLACK,
+        surrounding_alpha: float = 0.5,
+        **kwargs
+    ) -> TimeRange:
+        '''
+        添加字幕
+
+        - 文字可以传入一个列表，纵向排列显示
+        - 可以指定在当前位置往后 ``delay`` 秒才显示
+        - ``duration`` 表示持续时间
+        - ``scale`` 表示对文字的缩放，默认为 ``0.8``，可以传入列表表示对各个文字的缩放
+        - ``use_typst_text`` 表示是否使用 :class:`TypstText`，可以传入列表表示各个文字是否使用
+
+        返回值表示显示的时间段
+        '''
+        text_lst = [text] if isinstance(text, str) else text
+        scale_lst = [scale] if not isinstance(scale, Iterable) else scale
+        use_typst_lst = [use_typst_text] if not isinstance(use_typst_text, Iterable) else use_typst_text
+
+        if isinstance(duration, TimeRange):
+            range = duration
+        else:
+            range = TimeRange(self.current_time + delay, duration)
+
+        for text, scale, use_typst_text in zip(reversed(text_lst),
+                                               reversed(resize_preserving_order(scale_lst, len(text_lst))),
+                                               reversed(resize_preserving_order(use_typst_lst, len(text_lst)))):
+            subtitle = (TypstText if use_typst_text else Text)(text, **kwargs)
+            subtitle.depth.set(-1e5)
+            subtitle.points.scale(scale * base_scale)
+            self.place_subtitle(subtitle, range)
+            self.subtitle_infos.append(Timeline.SubtitleInfo(text,
+                                                             range,
+                                                             kwargs,
+                                                             subtitle))
+
+            subtitle_group = Group(
+                SurroundingRect(subtitle,
+                                color=surrounding_color,
+                                stroke_alpha=0,
+                                fill_alpha=surrounding_alpha),
+                subtitle
+            )
+            subtitle_group.depth.arrange(subtitle.depth.get())
+
+            self.schedule(range.at, subtitle_group.show)
+            self.schedule(range.end, subtitle_group.hide)
+
+        return range.copy()
+
+    def place_subtitle(self, subtitle: Text, range: TimeRange) -> None:
+        '''
+        被 :meth:`subtitle` 调用以将字幕放置到合适的位置：
+
+        - 对于同一批添加的字幕 ``[a, b]``，则 ``a`` 放在 ``b`` 的上面
+        - 如果在上文所述的 ``[a, b]`` 仍存在时，又加入了一个 ``c``，则 ``c`` 放在最上面
+        '''
+        for other in reversed(self.subtitle_infos):
+            # 根据 TimelineView 中排列显示标签的经验
+            # 这里加了一个 np.isclose 的判断
+            # 如果不加可能导致前一个字幕消失但是后一个字幕凭空出现在更上面
+            # （但是我没有测试过是否会出现这个bug，只是根据写 TimelineView 时的经验加了 np.isclose）
+            if other.range.at <= range.at < other.range.end and not np.isclose(range.at, other.range.end):
+                subtitle.points.next_to(other.subtitle, UP, buff=SMALL_BUFF)
+                return
+        subtitle.points.to_border(DOWN)
+
+    # endregion
+
+    # endregion
+
+    # region history
+
+    def track(self, item: Item) -> None:
+        '''
+        使得 ``item`` 在每次 ``forward`` 和 ``play`` 时都会被自动调用 :meth:`~.Item.detect_change`
+        '''
+        self.items_history[item]
+
+    def detect_changes_of_all(self) -> None:
+        '''
+        检查所有物件是否有产生变化并记录
+        '''
+        for item, ih in self.items_history.items():
+            self._detect_change(item, ih, as_time=self.current_time)
+
+    def detect_changes(self, items: Iterable[Item], *, as_time: float | None = None) -> None:
+        '''
+        检查指定的列表中的物件是否有产生变化并记录（仅检查自身而不包括子物件的）
+        '''
+        if as_time is None:
+            as_time = self.current_time
+        for item in items:
+            self._detect_change(item, self.items_history[item], as_time=as_time)
+
+    @staticmethod
+    def _detect_change(item: Item, ih: ItemHistory, *, as_time: float) -> None:
+        history_wo_dnmc = ih.history_without_dynamic
+        if not history_wo_dnmc.has_record() or not history_wo_dnmc.latest().data.not_changed(item):
+            item_copy = item.store()
+            ih.history.record_as_time(as_time, item_copy)
+            history_wo_dnmc.record_as_time(as_time, item_copy)
+
+    def register_dynamic(
+        self,
+        item: Item,
+        dynamic: DynamicItem,
+        static: Item | None,
+        begin: float,
+        end: float,
+        static_replaceable: bool
+    ) -> None:
+        ih = self.items_history[item]
+        ih.history.record_as_time(begin, dynamic)
+
+        if static is None:
+            if ih.history_without_dynamic.has_record():
+                static = ih.history_without_dynamic.latest().data
+            else:
+                static = item.store()
+        ih.history.record_as_time(end, static, replaceable=static_replaceable)
+        ih.history_without_dynamic.record_as_time(end, static, replaceable=static_replaceable)
+
+    def item_current[T](self, item: T, *, as_time: float | None = None, skip_dynamic=False) -> T:
+        '''
+        另见 :meth:`~.Item.current`
+        '''
+        ih = self.items_history[item]
+        history = ih.history_without_dynamic if skip_dynamic else ih.history
+        if not history.has_record():
+            return item
+
+        if as_time is None:
+            params = updater_params_ctx.get(None)
+            if params is not None:
+                as_time = params.global_t
+        if as_time is None:
+            as_time = Animation.global_t_ctx.get(None)
+
+        if as_time is None:
+            return item
+
+        item_or_dynamic = history.get(as_time)
+        return item_or_dynamic if isinstance(item_or_dynamic, Item) else item_or_dynamic(as_time)
+
+    # endregion
+
+    # region lineno
+
+    def get_construct_lineno(self) -> int | None:
+        '''
+        得到当前在 :meth:`construct` 中执行到的行数
+        '''
+        frame = inspect.currentframe().f_back
+        while frame is not None:
+            f_back = frame.f_back
+
+            if f_back is self._build_frame:
+                return frame.f_lineno
+
+            frame = f_back
+
+        return None     # pragma: no cover
+
+    def get_lineno_at_time(self, time: float):
+        '''
+        根据 ``time`` 得到对应执行到的行数
+        '''
+        times_of_code = self.times_of_code
+        if not times_of_code:
+            return -1
+
+        idx = bisect(times_of_code, time, key=lambda x: x.time)
+        idx = clip(idx, 0, len(times_of_code) - 1)
+        return times_of_code[idx].line
+
+    # endregion
+
+    # region debug
+
+    @staticmethod
+    def fmt_time(t: float) -> str:
+        time = round(t, 3)
+
+        minutes = int(time // 60)
+        time %= 60
+
+        hours = minutes // 60
+        minutes %= 60
+
+        seconds = math.floor(time)
+        ms = round((time - seconds) * 1e3)
+
+        times = []
+        if hours != 0:
+            times.append(f'{hours}h')
+        times.append(f'{minutes:>3d}m' if minutes != 0 else ' ' * 4)
+        times.append(f'{seconds:>3d}s')
+        times.append(f'{ms:>4d}ms' if ms != 0 else ' ' * 6)
+
+        return "".join(times)
+
+    def dbg_time(self, ext_msg: str = '') -> None:  # pragma: no cover
+        if ext_msg:
+            ext_msg = f'[{ext_msg}]  '
+
+        time = self.fmt_time(self.current_time)
+
+        log.debug(f't={time}  {ext_msg}at construct.{self.get_construct_lineno()}')
+
+    # endregion
+
+
+class SourceTimeline(Timeline):     # pragma: no cover
+    '''
+    与 :class:`Timeline` 相比，会在背景显示源代码
+    '''
+    def build(self, *, quiet=False) -> TimelineAnim:
+        from janim.items.text.text import SourceDisplayer
+        with ContextSetter(self.ctx_var, self):
+            SourceDisplayer(self.__class__).show()
+        return super().build(quiet=quiet)
+
+
+class TimelineAnim(AnimGroup):
+    '''
+    运行 :meth:`Timeline.run` 后返回的动画组
+
+    - ``self.display_anim`` 是由 :meth:`Timeline.construct` 中执行
+      :meth:`Timeline.show` 和 :meth:`Timeline.hide` 而产生的
+    - ``self.user_anim`` 是显式使用了 :meth:`Timeline.prepare` 或 :meth:`Timeline.play` 而产生的
+    '''
+    def __init__(self, timeline: Timeline, **kwargs):
+        self.timeline = timeline
+
+        self.display_anim = AnimGroup(*timeline.display_anims)
+        self.user_anim = AnimGroup(*timeline.anims)
+        super().__init__(self.display_anim, self.user_anim, **kwargs)
+        self.maxt = self.local_range.duration = timeline.current_time
+
+        self.display_anim.global_range = self.display_anim.local_range
+        self.user_anim.global_range = self.user_anim.local_range
+        self.global_range = self.local_range
+
+        self.flattened = self.flatten()
+        self._time: float | None = None
+
+    @property
+    def cfg(self) -> Config | ConfigGetter:
+        return self.timeline.config_getter
+
+    def anim_on(self, local_t: float) -> None:
+        # 使最后一帧不空屏
+        if np.isclose(local_t, self.global_range.duration):
+            local_t -= 1 / self.cfg.fps
+
+        self._time = local_t
+        with ContextSetter(self.global_t_ctx, local_t):
+            super().anim_on(local_t)
+
+    def render_all(self, ctx: mgl.Context) -> None:
+        '''
+        调用所有的 :class:`RenderCall` 进行渲染
+        '''
+        if self._time is None:
+            return
+
+        try:
+            with ContextSetter(Animation.global_t_ctx, self._time):
+                timeline = self.timeline
+                camera_info = timeline.camera.current().points.info
+                anti_alias_radius = self.cfg.anti_alias_width / 2 * camera_info.scaled_factor
+
+                set_global_uniforms(
+                    ctx,
+                    ('JA_VIEW_MATRIX', camera_info.view_matrix.T.flatten()),
+                    ('JA_PROJ_MATRIX', camera_info.proj_matrix.T.flatten()),
+                    ('JA_FRAME_RADIUS', camera_info.frame_radius),
+                    ('JA_ANTI_ALIAS_RADIUS', anti_alias_radius)
+                )
+
+                with ContextSetter(Renderer.data_ctx, RenderData(ctx=ctx,
+                                                                 camera_info=camera_info,
+                                                                 anti_alias_radius=anti_alias_radius)):
+                    # 使用 heapq 以深度为序调用 RenderCall
+                    render_calls = heapq.merge(
+                        *[
+                            anim.render_call_list
+                            for anim in self.flattened
+                            if anim.render_call_list and anim.global_range.at <= self._time < anim.global_range.end
+                        ],
+                        key=lambda x: x.depth,
+                        reverse=True
+                    )
+                    for render_call in render_calls:
+                        render_call.func()
+
+        except Exception:
+            traceback.print_exc()
+
+    capture_ctx: mgl.Context | None = None
+    capture_fbo: mgl.Framebuffer | None = None
+
+    def capture(self) -> Image.Image:
+        if TimelineAnim.capture_ctx is None:
+            TimelineAnim.capture_ctx = mgl.create_standalone_context(require=430)
+            TimelineAnim.capture_ctx.enable(mgl.BLEND)
+            TimelineAnim.capture_ctx.blend_func = (
+                mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+                mgl.ONE, mgl.ONE
+            )
+            TimelineAnim.capture_ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
+
+            pw, ph = self.cfg.pixel_width, self.cfg.pixel_height
+            TimelineAnim.capture_fbo = TimelineAnim.capture_ctx.framebuffer(
+                color_attachments=TimelineAnim.capture_ctx.texture(
+                    (pw, ph),
+                    components=4,
+                    samples=0,
+                ),
+                depth_attachment=TimelineAnim.capture_ctx.depth_renderbuffer(
+                    (pw, ph),
+                    samples=0
+                )
+            )
+
+        fbo = TimelineAnim.capture_fbo
+        fbo.use()
+        fbo.clear(*self.cfg.background_color.rgb)
+        self.render_all(TimelineAnim.capture_ctx)
+
+        return Image.frombytes(
+            "RGBA", fbo.size, fbo.read(components=4),
+            "raw", "RGBA", 0, -1
+        )
```

### Comparing `janim-1.0.4/janim/anims/updater.py` & `janim-1.1.0/janim/anims/updater.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,279 +1,279 @@
-from __future__ import annotations
-
-import inspect
-from contextvars import ContextVar
-from dataclasses import dataclass
-from typing import Any, Callable, Self
-
-from janim.anims.animation import Animation, RenderCall, TimeRange
-from janim.constants import ANIM_END_DELTA, C_LABEL_ANIM_ABSTRACT
-from janim.exception import UpdaterError
-from janim.items.item import DynamicItem, Item
-from janim.utils.simple_functions import clip
-
-
-@dataclass
-class UpdaterParams:
-    '''
-    ``Updater`` 调用时会传递的参数，用于标注时间信息以及动画进度
-    '''
-    updater: DataUpdater | ItemUpdater
-    global_t: float
-    alpha: float
-    range: TimeRange
-    extra_data: tuple | None
-
-    def __enter__(self) -> Self:
-        self.token = updater_params_ctx.set(self)
-        return self
-
-    def __exit__(self, exc_type, exc_value, tb):
-        updater_params_ctx.reset(self.token)
-
-
-updater_params_ctx: ContextVar[UpdaterParams] = ContextVar('updater_params_ctx')
-
-type DataUpdaterFn[T] = Callable[[T, UpdaterParams], Any]
-
-
-class DataUpdater[T: Item](Animation):
-    '''
-    以时间为参数对物件的数据进行修改
-
-    例如：
-
-    .. code-block:: python
-
-        class Example(Timeline):
-            def construct(self) -> None:
-                rect = Rect()
-                rect.points.to_border(LEFT)
-
-                self.play(
-                    DataUpdater(
-                        rect,
-                        lambda data, p: data.points.rotate(p.alpha * 180 * DEGREES).shift(p.alpha * 6 * RIGHT)
-                    )
-                )
-
-    会产生一个“矩形从左侧旋转着移动到右侧”的动画
-
-    另见：:class:`~.UpdaterExample`
-    '''
-    label_color = C_LABEL_ANIM_ABSTRACT
-
-    @dataclass
-    class DataGroup:
-        orig_data: Item
-        data: Item
-        extra_data: Any | None
-
-    def __init__(
-        self,
-        item: T,
-        func: DataUpdaterFn[T],
-        *,
-        lag_ratio: float = 0,
-        hide_at_begin: bool = True,
-        show_at_end: bool = True,
-        become_at_end: bool = True,
-        skip_null_items: bool = True,
-        root_only: bool = True,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.item = item
-        self.func = func
-        self.lag_ratio = lag_ratio
-        self.hide_at_begin = hide_at_begin
-        self.show_at_end = show_at_end
-        self.become_at_end = become_at_end
-        self.skip_null_items = skip_null_items
-        self.root_only = root_only
-
-        self.post_updaters: list[DataUpdaterFn[T]] = []
-
-        for subitem in item.walk_self_and_descendants(root_only):
-            self.timeline.track(subitem)
-
-    def add_post_updater(self, updater: DataUpdaterFn[T]) -> Self:
-        self.post_updaters.append(updater)
-        return self
-
-    def call(self, data: T, p: UpdaterParams) -> None:
-        self.func(data, p)
-        for updater in self.post_updaters:
-            updater(data, p)
-
-    def create_extra_data(self, data: Item) -> Any | None:
-        return None
-
-    def wrap_dynamic(self, updater_data: DataUpdater.DataGroup) -> DynamicItem:
-        '''
-        以供传入 :meth:`~.Timeline.register_dynamic_data` 使用
-        '''
-        def wrapper(global_t: float) -> Item:
-            alpha = self.get_alpha_on_global_t(global_t)
-            data_copy = updater_data.orig_data.store()
-
-            with UpdaterParams(self,
-                               global_t,
-                               alpha,
-                               self.global_range,
-                               updater_data.extra_data) as params:
-                self.call(data_copy, params)
-
-            return data_copy
-
-        return wrapper
-
-    def anim_init(self) -> None:
-        def build_data(data: Item) -> DataUpdater.DataGroup:
-            return DataUpdater.DataGroup(data, data.store(), self.create_extra_data(data))
-
-        self.datas: dict[Item, DataUpdater.DataGroup] = {
-            item: build_data(
-                item.current(as_time=self.global_range.at,
-                             skip_dynamic=True)
-            )
-            for item in self.item.walk_self_and_descendants(self.root_only)
-            if not self.skip_null_items or not item.is_null()
-        }
-
-        for item, updater_data in self.datas.items():
-            if self.become_at_end:
-                with UpdaterParams(self,
-                                   self.global_range.end,
-                                   1,
-                                   self.global_range,
-                                   updater_data.extra_data) as params:
-                    self.call(item, params)
-
-            self.timeline.register_dynamic(item,
-                                           self.wrap_dynamic(updater_data),
-                                           item.store() if self.become_at_end else None,
-                                           self.global_range.at,
-                                           self.global_range.end - ANIM_END_DELTA,
-                                           not self.become_at_end)
-
-        self.set_render_call_list([
-            RenderCall(
-                updater_data.data.depth,
-                updater_data.data.render
-            )
-            for updater_data in self.datas.values()
-        ])
-
-        # 在动画开始时自动隐藏，在动画结束时自动显示
-        # 可以将 ``hide_on_begin`` 和 ``show_on_end`` 置为 ``False`` 以禁用
-        if self.hide_at_begin:
-            self.timeline.schedule(self.global_range.at, self.item.hide, root_only=self.root_only)
-        if self.show_at_end:
-            self.timeline.schedule(self.global_range.end, self.item.show, root_only=self.root_only)
-
-    def anim_on_alpha(self, alpha: float) -> None:
-        global_t = self.global_t_ctx.get()
-        for i, updater_data in enumerate(self.datas.values()):
-            sub_alpha = self.get_sub_alpha(alpha, i)
-            updater_data.data.restore(updater_data.orig_data)
-
-            with UpdaterParams(self,
-                               global_t,
-                               sub_alpha,
-                               self.global_range,
-                               updater_data.extra_data) as params:
-                self.call(updater_data.data, params)
-
-    def get_sub_alpha(
-        self,
-        alpha: float,
-        index: int
-    ) -> float:
-        '''依据 ``lag_ratio`` 得到特定子物件的 ``sub_alpha``'''
-        # REFACTOR: make this more understanable
-        lag_ratio = self.lag_ratio
-        full_length = (len(self.datas) - 1) * lag_ratio + 1
-        value = alpha * full_length
-        lower = index * lag_ratio
-        return clip((value - lower), 0, 1)
-
-
-# TODO: optimize
-class ItemUpdater(Animation):
-    '''
-    以时间为参数显示物件
-
-    也就是说，在 :class:`ItemUpdater` 执行时，对于每帧，都会执行 ``func``，并显示 ``func`` 返回的物件
-
-    在默认情况下：
-
-    - 传入的 ``item`` 会在动画的末尾被替换为动画最后一帧 ``func`` 所返回的物件，传入 ``become_at_end=False`` 以禁用
-    - 传入的 ``item`` 会在动画开始时隐藏，在动画结束后显示，传入 ``hide_at_begin=False`` 和 ``show_at_end=False`` 以禁用
-    - 若传入 ``item=None``，则以上两点都无效
-
-    另见：:class:`~.UpdaterExample`
-    '''
-    label_color = C_LABEL_ANIM_ABSTRACT
-
-    def __init__(
-        self,
-        item: Item | None,
-        func: Callable[[UpdaterParams], Item],
-        *,
-        hide_at_begin: bool = True,
-        show_at_end: bool = True,
-        become_at_end: bool = True,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.func = func
-        self.item = item
-        self.hide_at_begin = hide_at_begin
-        self.show_at_end = show_at_end
-        self.become_at_end = become_at_end
-
-    def call(self, p: UpdaterParams) -> Item:
-        ret = self.func(p)
-        if not isinstance(ret, Item):
-            raise UpdaterError(f'传入 ItemUpdater 的函数必须以一个物件作为返回值，而返回的是 {ret}，'
-                               f'函数定义于 {inspect.getfile(self.func)}:{inspect.getsourcelines(self.func)[1]}')
-        for item in ret.walk_self_and_descendants():
-            item.is_temporary = True
-        return ret
-
-    def anim_init(self) -> None:
-        if self.item is None:
-            return
-
-        # 在动画开始时自动隐藏，在动画结束时自动显示
-        # 可以将 ``hide_on_begin`` 和 ``show_on_end`` 置为 ``False`` 以禁用
-        if self.hide_at_begin:
-            self.timeline.schedule(self.global_range.at, self.item.hide)
-        if self.show_at_end:
-            self.timeline.schedule(self.global_range.end, self.item.show)
-
-        # 在动画结束后，自动使用动画最后一帧的物件替换原有的
-        if self.become_at_end:
-            self.timeline.schedule(self.global_range.end, self.scheduled_become)
-
-    def scheduled_become(self) -> None:
-        with UpdaterParams(self,
-                           self.global_range.end,
-                           1,
-                           self.global_range,
-                           None) as params:
-            self.item.become(self.call(params))
-
-    def anim_on_alpha(self, alpha: float) -> None:
-        global_t = self.global_t_ctx.get()
-
-        with UpdaterParams(self, global_t, alpha, self.global_range, None) as params:
-            dynamic = self.call(params)
-
-        self.set_render_call_list([
-            RenderCall(
-                sub.depth,
-                sub.render
-            )
-            for sub in dynamic.walk_self_and_descendants()
-        ])
+from __future__ import annotations
+
+import inspect
+from contextvars import ContextVar
+from dataclasses import dataclass
+from typing import Any, Callable, Self
+
+from janim.anims.animation import Animation, RenderCall, TimeRange
+from janim.constants import ANIM_END_DELTA, C_LABEL_ANIM_ABSTRACT
+from janim.exception import UpdaterError
+from janim.items.item import DynamicItem, Item
+from janim.utils.simple_functions import clip
+
+
+@dataclass
+class UpdaterParams:
+    '''
+    ``Updater`` 调用时会传递的参数，用于标注时间信息以及动画进度
+    '''
+    updater: DataUpdater | ItemUpdater
+    global_t: float
+    alpha: float
+    range: TimeRange
+    extra_data: tuple | None
+
+    def __enter__(self) -> Self:
+        self.token = updater_params_ctx.set(self)
+        return self
+
+    def __exit__(self, exc_type, exc_value, tb):
+        updater_params_ctx.reset(self.token)
+
+
+updater_params_ctx: ContextVar[UpdaterParams] = ContextVar('updater_params_ctx')
+
+type DataUpdaterFn[T] = Callable[[T, UpdaterParams], Any]
+
+
+class DataUpdater[T: Item](Animation):
+    '''
+    以时间为参数对物件的数据进行修改
+
+    例如：
+
+    .. code-block:: python
+
+        class Example(Timeline):
+            def construct(self) -> None:
+                rect = Rect()
+                rect.points.to_border(LEFT)
+
+                self.play(
+                    DataUpdater(
+                        rect,
+                        lambda data, p: data.points.rotate(p.alpha * 180 * DEGREES).shift(p.alpha * 6 * RIGHT)
+                    )
+                )
+
+    会产生一个“矩形从左侧旋转着移动到右侧”的动画
+
+    另见：:class:`~.UpdaterExample`
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
+    @dataclass
+    class DataGroup:
+        orig_data: Item
+        data: Item
+        extra_data: Any | None
+
+    def __init__(
+        self,
+        item: T,
+        func: DataUpdaterFn[T],
+        *,
+        lag_ratio: float = 0,
+        hide_at_begin: bool = True,
+        show_at_end: bool = True,
+        become_at_end: bool = True,
+        skip_null_items: bool = True,
+        root_only: bool = True,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        self.item = item
+        self.func = func
+        self.lag_ratio = lag_ratio
+        self.hide_at_begin = hide_at_begin
+        self.show_at_end = show_at_end
+        self.become_at_end = become_at_end
+        self.skip_null_items = skip_null_items
+        self.root_only = root_only
+
+        self.post_updaters: list[DataUpdaterFn[T]] = []
+
+        for subitem in item.walk_self_and_descendants(root_only):
+            self.timeline.track(subitem)
+
+    def add_post_updater(self, updater: DataUpdaterFn[T]) -> Self:
+        self.post_updaters.append(updater)
+        return self
+
+    def call(self, data: T, p: UpdaterParams) -> None:
+        self.func(data, p)
+        for updater in self.post_updaters:
+            updater(data, p)
+
+    def create_extra_data(self, data: Item) -> Any | None:
+        return None
+
+    def wrap_dynamic(self, updater_data: DataUpdater.DataGroup) -> DynamicItem:
+        '''
+        以供传入 :meth:`~.Timeline.register_dynamic` 使用
+        '''
+        def wrapper(global_t: float) -> Item:
+            alpha = self.get_alpha_on_global_t(global_t)
+            data_copy = updater_data.orig_data.store()
+
+            with UpdaterParams(self,
+                               global_t,
+                               alpha,
+                               self.global_range,
+                               updater_data.extra_data) as params:
+                self.call(data_copy, params)
+
+            return data_copy
+
+        return wrapper
+
+    def anim_init(self) -> None:
+        def build_data(data: Item) -> DataUpdater.DataGroup:
+            return DataUpdater.DataGroup(data, data.store(), self.create_extra_data(data))
+
+        self.datas: dict[Item, DataUpdater.DataGroup] = {
+            item: build_data(
+                item.current(as_time=self.global_range.at,
+                             skip_dynamic=True)
+            )
+            for item in self.item.walk_self_and_descendants(self.root_only)
+            if not self.skip_null_items or not item.is_null()
+        }
+
+        for item, updater_data in self.datas.items():
+            if self.become_at_end:
+                with UpdaterParams(self,
+                                   self.global_range.end,
+                                   1,
+                                   self.global_range,
+                                   updater_data.extra_data) as params:
+                    self.call(item, params)
+
+            self.timeline.register_dynamic(item,
+                                           self.wrap_dynamic(updater_data),
+                                           item.store() if self.become_at_end else None,
+                                           self.global_range.at,
+                                           self.global_range.end - ANIM_END_DELTA,
+                                           not self.become_at_end)
+
+        self.set_render_call_list([
+            RenderCall(
+                updater_data.data.depth,
+                updater_data.data.render
+            )
+            for updater_data in self.datas.values()
+        ])
+
+        # 在动画开始时自动隐藏，在动画结束时自动显示
+        # 可以将 ``hide_on_begin`` 和 ``show_on_end`` 置为 ``False`` 以禁用
+        if self.hide_at_begin:
+            self.timeline.schedule(self.global_range.at, self.item.hide, root_only=self.root_only)
+        if self.show_at_end:
+            self.timeline.schedule(self.global_range.end, self.item.show, root_only=self.root_only)
+
+    def anim_on_alpha(self, alpha: float) -> None:
+        global_t = self.global_t_ctx.get()
+        for i, updater_data in enumerate(self.datas.values()):
+            sub_alpha = self.get_sub_alpha(alpha, i)
+            updater_data.data.restore(updater_data.orig_data)
+
+            with UpdaterParams(self,
+                               global_t,
+                               sub_alpha,
+                               self.global_range,
+                               updater_data.extra_data) as params:
+                self.call(updater_data.data, params)
+
+    def get_sub_alpha(
+        self,
+        alpha: float,
+        index: int
+    ) -> float:
+        '''依据 ``lag_ratio`` 得到特定子物件的 ``sub_alpha``'''
+        # REFACTOR: make this more understanable
+        lag_ratio = self.lag_ratio
+        full_length = (len(self.datas) - 1) * lag_ratio + 1
+        value = alpha * full_length
+        lower = index * lag_ratio
+        return clip((value - lower), 0, 1)
+
+
+# TODO: optimize
+class ItemUpdater(Animation):
+    '''
+    以时间为参数显示物件
+
+    也就是说，在 :class:`ItemUpdater` 执行时，对于每帧，都会执行 ``func``，并显示 ``func`` 返回的物件
+
+    在默认情况下：
+
+    - 传入的 ``item`` 会在动画的末尾被替换为动画最后一帧 ``func`` 所返回的物件，传入 ``become_at_end=False`` 以禁用
+    - 传入的 ``item`` 会在动画开始时隐藏，在动画结束后显示，传入 ``hide_at_begin=False`` 和 ``show_at_end=False`` 以禁用
+    - 若传入 ``item=None``，则以上两点都无效
+
+    另见：:class:`~.UpdaterExample`
+    '''
+    label_color = C_LABEL_ANIM_ABSTRACT
+
+    def __init__(
+        self,
+        item: Item | None,
+        func: Callable[[UpdaterParams], Item],
+        *,
+        hide_at_begin: bool = True,
+        show_at_end: bool = True,
+        become_at_end: bool = True,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        self.func = func
+        self.item = item
+        self.hide_at_begin = hide_at_begin
+        self.show_at_end = show_at_end
+        self.become_at_end = become_at_end
+
+    def call(self, p: UpdaterParams) -> Item:
+        ret = self.func(p)
+        if not isinstance(ret, Item):
+            raise UpdaterError(f'传入 ItemUpdater 的函数必须以一个物件作为返回值，而返回的是 {ret}，'
+                               f'函数定义于 {inspect.getfile(self.func)}:{inspect.getsourcelines(self.func)[1]}')
+        for item in ret.walk_self_and_descendants():
+            item.is_temporary = True
+        return ret
+
+    def anim_init(self) -> None:
+        if self.item is None:
+            return
+
+        # 在动画开始时自动隐藏，在动画结束时自动显示
+        # 可以将 ``hide_on_begin`` 和 ``show_on_end`` 置为 ``False`` 以禁用
+        if self.hide_at_begin:
+            self.timeline.schedule(self.global_range.at, self.item.hide)
+        if self.show_at_end:
+            self.timeline.schedule(self.global_range.end, self.item.show)
+
+        # 在动画结束后，自动使用动画最后一帧的物件替换原有的
+        if self.become_at_end:
+            self.timeline.schedule(self.global_range.end, self.scheduled_become)
+
+    def scheduled_become(self) -> None:
+        with UpdaterParams(self,
+                           self.global_range.end,
+                           1,
+                           self.global_range,
+                           None) as params:
+            self.item.become(self.call(params))
+
+    def anim_on_alpha(self, alpha: float) -> None:
+        global_t = self.global_t_ctx.get()
+
+        with UpdaterParams(self, global_t, alpha, self.global_range, None) as params:
+            dynamic = self.call(params)
+
+        self.set_render_call_list([
+            RenderCall(
+                sub.depth,
+                sub.render
+            )
+            for sub in dynamic.walk_self_and_descendants()
+        ])
```

### Comparing `janim-1.0.4/janim/camera/camera.py` & `janim-1.1.0/janim/camera/camera.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from __future__ import annotations
-
-from typing import Iterable, Self
-
-import numpy as np
-from scipy.spatial.transform import Rotation, Slerp
-
-import janim.utils.refresh as refresh
-from janim.camera.camera_info import CameraInfo
-from janim.components.component import CmptInfo
-from janim.components.points import Cmpt_Points
-from janim.constants import ORIGIN, OUT
-from janim.items.points import Points
-from janim.typing import Vect
-from janim.utils.bezier import interpolate
-from janim.utils.config import Config
-from janim.utils.paths import PathFunc, straight_path
-from janim.utils.simple_functions import clip
-from janim.utils.space_ops import normalize
-
-
-class Cmpt_CameraPoints[ItemT](Cmpt_Points[ItemT]):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.reset()
-
-    def reset(self) -> Self:
-        '''
-        将摄像机几何属性设置为初始状态
-        '''
-        self.orig_height = Config.get.frame_height
-
-        self.set([ORIGIN])
-        self.size = [Config.get.frame_width, Config.get.frame_height]
-        self.fov = 45
-        self.orientation = Rotation.identity()
-
-        return self
-
-    def copy(self) -> Self:
-        cmpt_copy = super().copy()
-        cmpt_copy._size = self._size.copy()
-        cmpt_copy.orientation = self.orientation.from_quat(self.orientation.as_quat())
-        return cmpt_copy
-
-    def become(self, other: Cmpt_CameraPoints) -> Self:
-        self.set(other.get())
-        self.size = other.size
-        self.fov = other.fov
-        # 有无更好的复制方法？
-        self.orientation = Rotation.from_rotvec(other.orientation.as_rotvec())
-
-        return self
-
-    def not_changed(self, other: Cmpt_CameraPoints) -> Self:
-        if not super().not_changed(other):
-            return False
-        if np.any(self.size != other.size) or self.fov != other.fov:
-            return False
-        return np.all(self.orientation.as_quat() == other.orientation.as_quat())
-
-    def interpolate(
-        self,
-        cmpt1: Self,
-        cmpt2: Self,
-        alpha: float,
-        *,
-        path_func: PathFunc = straight_path
-    ) -> None:
-        # 下面对 Slerp 的调用有次出现了 ValueError: Interpolation times must be within the range [0, 1], both inclusive.
-        # 所以这里限制一下 alpha（本来我觉得没必要的，但是为什么会有上面这个报错呢）
-        alpha = clip(alpha, 0, 1)
-
-        super().interpolate(cmpt1, cmpt2, alpha)
-        self.size = interpolate(cmpt1.size, cmpt2.size, alpha)
-        self.fov = interpolate(cmpt1.fov, cmpt2.fov, alpha)
-        self.orientation = Slerp([0, 1], Rotation.concatenate([cmpt1.orientation, cmpt2.orientation]))(alpha)
-
-    @property
-    def scaled_factor(self) -> float:
-        return self.size[1] / self.orig_height
-
-    @property
-    def size(self) -> np.ndarray:
-        return self._size
-
-    @size.setter
-    def size(self, value: Vect) -> None:
-        self._size = np.array(value)
-        self.mark_refresh(Cmpt_CameraPoints.info.fget)
-
-    @property
-    def fov(self) -> float:
-        return self._fov
-
-    @fov.setter
-    def fov(self, val: float) -> None:
-        self._fov = val
-        self.mark_refresh(Cmpt_CameraPoints.info.fget)
-
-    def scale(
-        self,
-        scale_factor: float | Iterable,
-        **kwargs
-    ) -> Self:
-        '''
-        将摄像机缩放指定倍数
-        '''
-        self._size *= scale_factor
-        return self
-
-    def rotate(
-        self,
-        angle: float,
-        *,
-        axis: Vect = OUT,
-        **kwargs
-    ) -> Self:
-        '''
-        将摄像机绕 ``axis`` 轴进行旋转
-        '''
-        super().rotate(angle, axis=axis, **kwargs)
-        self.orientation *= Rotation.from_rotvec(angle * normalize(axis))
-        return self
-
-    @property
-    @Cmpt_Points.set.self_refresh()
-    @refresh.register
-    def info(self) -> CameraInfo:
-        '''
-        摄像机的几何属性
-        '''
-        rot_mat_T = self.orientation.as_matrix().T
-        width, height = self.size
-        return CameraInfo(
-            self.scaled_factor,
-            self.fov,
-            self.self_box.center,
-            np.dot(np.array([width, 0, 0]), rot_mat_T),
-            np.dot(np.array([0, height, 0]), rot_mat_T)
-        )
-
-
-class Camera(Points):
-    points = CmptInfo(Cmpt_CameraPoints[Self])
+from __future__ import annotations
+
+from typing import Iterable, Self
+
+import numpy as np
+from scipy.spatial.transform import Rotation, Slerp
+
+import janim.utils.refresh as refresh
+from janim.camera.camera_info import CameraInfo
+from janim.components.component import CmptInfo
+from janim.components.points import Cmpt_Points
+from janim.constants import ORIGIN, OUT
+from janim.items.points import Points
+from janim.typing import Vect
+from janim.utils.bezier import interpolate
+from janim.utils.config import Config
+from janim.utils.paths import PathFunc, straight_path
+from janim.utils.simple_functions import clip
+from janim.utils.space_ops import normalize
+
+
+class Cmpt_CameraPoints[ItemT](Cmpt_Points[ItemT]):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.reset()
+
+    def reset(self) -> Self:
+        '''
+        将摄像机几何属性设置为初始状态
+        '''
+        self.orig_height = Config.get.frame_height
+
+        self.set([ORIGIN])
+        self.size = [Config.get.frame_width, Config.get.frame_height]
+        self.fov = 45
+        self.orientation = Rotation.identity()
+
+        return self
+
+    def copy(self) -> Self:
+        cmpt_copy = super().copy()
+        cmpt_copy._size = self._size.copy()
+        cmpt_copy.orientation = self.orientation.from_quat(self.orientation.as_quat())
+        return cmpt_copy
+
+    def become(self, other: Cmpt_CameraPoints) -> Self:
+        self.set(other.get())
+        self.size = other.size
+        self.fov = other.fov
+        # 有无更好的复制方法？
+        self.orientation = Rotation.from_rotvec(other.orientation.as_rotvec())
+
+        return self
+
+    def not_changed(self, other: Cmpt_CameraPoints) -> Self:
+        if not super().not_changed(other):
+            return False
+        if np.any(self.size != other.size) or self.fov != other.fov:
+            return False
+        return np.all(self.orientation.as_quat() == other.orientation.as_quat())
+
+    def interpolate(
+        self,
+        cmpt1: Self,
+        cmpt2: Self,
+        alpha: float,
+        *,
+        path_func: PathFunc = straight_path
+    ) -> None:
+        # 下面对 Slerp 的调用有次出现了 ValueError: Interpolation times must be within the range [0, 1], both inclusive.
+        # 所以这里限制一下 alpha（本来我觉得没必要的，但是为什么会有上面这个报错呢）
+        alpha = clip(alpha, 0, 1)
+
+        super().interpolate(cmpt1, cmpt2, alpha)
+        self.size = interpolate(cmpt1.size, cmpt2.size, alpha)
+        self.fov = interpolate(cmpt1.fov, cmpt2.fov, alpha)
+        self.orientation = Slerp([0, 1], Rotation.concatenate([cmpt1.orientation, cmpt2.orientation]))(alpha)
+
+    @property
+    def scaled_factor(self) -> float:
+        return self.size[1] / self.orig_height
+
+    @property
+    def size(self) -> np.ndarray:
+        return self._size
+
+    @size.setter
+    def size(self, value: Vect) -> None:
+        self._size = np.array(value)
+        self.mark_refresh(Cmpt_CameraPoints.info.fget)
+
+    @property
+    def fov(self) -> float:
+        return self._fov
+
+    @fov.setter
+    def fov(self, val: float) -> None:
+        self._fov = val
+        self.mark_refresh(Cmpt_CameraPoints.info.fget)
+
+    def scale(
+        self,
+        scale_factor: float | Iterable,
+        **kwargs
+    ) -> Self:
+        '''
+        将摄像机缩放指定倍数
+        '''
+        self._size *= scale_factor
+        return self
+
+    def rotate(
+        self,
+        angle: float,
+        *,
+        axis: Vect = OUT,
+        **kwargs
+    ) -> Self:
+        '''
+        将摄像机绕 ``axis`` 轴进行旋转
+        '''
+        super().rotate(angle, axis=axis, **kwargs)
+        self.orientation *= Rotation.from_rotvec(angle * normalize(axis))
+        return self
+
+    @property
+    @Cmpt_Points.set.self_refresh()
+    @refresh.register
+    def info(self) -> CameraInfo:
+        '''
+        摄像机的几何属性
+        '''
+        rot_mat_T = self.orientation.as_matrix().T
+        width, height = self.size
+        return CameraInfo(
+            self.scaled_factor,
+            self.fov,
+            self.self_box.center,
+            np.dot(np.array([width, 0, 0]), rot_mat_T),
+            np.dot(np.array([0, height, 0]), rot_mat_T)
+        )
+
+
+class Camera(Points):
+    points = CmptInfo(Cmpt_CameraPoints[Self])
```

### Comparing `janim-1.0.4/janim/camera/camera_info.py` & `janim-1.1.0/janim/camera/camera_info.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-import math
-from dataclasses import dataclass, field
-
-import numpy as np
-
-from janim.utils.space_ops import get_norm, normalize, get_unit_normal
-from janim.typing import VectArray
-
-
-@dataclass
-class CameraInfo:
-    scaled_factor: float
-
-    fov: float
-    center: np.ndarray
-    horizontal_vect: np.ndarray
-    vertical_vect: np.ndarray
-
-    horizontal_dist: float = field(init=False)
-    vertical_dist: float = field(init=False)
-
-    camera_location: np.ndarray = field(init=False)
-
-    view_matrix: np.ndarray = field(init=False)
-    proj_matrix: np.ndarray = field(init=False)
-    proj_view_matrix: np.ndarray = field(init=False)
-    frame_radius: np.ndarray = field(init=False)
-
-    def __post_init__(self):
-        self.horizontal_dist = get_norm(self.horizontal_vect)
-        self.vertical_dist = get_norm(self.vertical_vect)
-
-        self.camera_location = self._compute_camera_location()
-
-        self.view_matrix = self._compute_view_matrix()
-        self.proj_matrix = self._compute_proj_matrix()
-        self.proj_view_matrix = np.dot(self.proj_matrix, self.view_matrix)
-        self.frame_radius = np.array([self.horizontal_dist, self.vertical_dist]) / 2
-
-    @property
-    def frame_size(self) -> tuple[float, float]:
-        return self.horizontal_dist, self.vertical_dist
-
-    def map_points(self, points: VectArray) -> np.ndarray:
-        aligned = np.hstack([
-            points,
-            np.full((len(points), 1), 1)
-        ])
-        mapped = np.dot(aligned, self.proj_view_matrix.T)
-        return mapped[:, :2] / mapped[:, 3].reshape((len(mapped), 1))
-
-    def _compute_camera_location(self) -> np.ndarray:
-        right = self.horizontal_vect
-        up = self.vertical_vect
-        normal = get_unit_normal(right, up)
-        distance = get_norm(up) / 2 / math.tan(math.radians(self.fov / 2))
-        return self.center + normal * distance
-
-    def _compute_view_matrix(self) -> np.ndarray:
-        rot_matrix = np.eye(4)
-        rot_matrix[0, :3] = normalize(self.horizontal_vect)
-        rot_matrix[1, :3] = normalize(self.vertical_vect)
-        rot_matrix[2, :3] = normalize(self.camera_location - self.center)
-
-        shift_matrix = np.eye(4)
-        shift_matrix[:3, 3] = -self.camera_location
-
-        return np.dot(rot_matrix, shift_matrix)
-
-    def _compute_proj_matrix(self, near=0.1, far=100.0) -> np.ndarray:
-        aspect = self.horizontal_dist / self.vertical_dist
-
-        f = 1.0 / np.tan(np.radians(self.fov) / 2.0)
-        return np.array([
-            [f / aspect, 0, 0, 0],
-            [0, f, 0, 0],
-            [0, 0, (far + near) / (near - far), 2 * far * near / (near - far)],
-            [0, 0, -1, 0]
-        ])
+import math
+from dataclasses import dataclass, field
+
+import numpy as np
+
+from janim.utils.space_ops import get_norm, normalize, get_unit_normal
+from janim.typing import VectArray
+
+
+@dataclass
+class CameraInfo:
+    scaled_factor: float
+
+    fov: float
+    center: np.ndarray
+    horizontal_vect: np.ndarray
+    vertical_vect: np.ndarray
+
+    horizontal_dist: float = field(init=False)
+    vertical_dist: float = field(init=False)
+
+    camera_location: np.ndarray = field(init=False)
+
+    view_matrix: np.ndarray = field(init=False)
+    proj_matrix: np.ndarray = field(init=False)
+    proj_view_matrix: np.ndarray = field(init=False)
+    frame_radius: np.ndarray = field(init=False)
+
+    def __post_init__(self):
+        self.horizontal_dist = get_norm(self.horizontal_vect)
+        self.vertical_dist = get_norm(self.vertical_vect)
+
+        self.camera_location = self._compute_camera_location()
+
+        self.view_matrix = self._compute_view_matrix()
+        self.proj_matrix = self._compute_proj_matrix()
+        self.proj_view_matrix = np.dot(self.proj_matrix, self.view_matrix)
+        self.frame_radius = np.array([self.horizontal_dist, self.vertical_dist]) / 2
+
+    @property
+    def frame_size(self) -> tuple[float, float]:
+        return self.horizontal_dist, self.vertical_dist
+
+    def map_points(self, points: VectArray) -> np.ndarray:
+        aligned = np.hstack([
+            points,
+            np.full((len(points), 1), 1)
+        ])
+        mapped = np.dot(aligned, self.proj_view_matrix.T)
+        return mapped[:, :2] / mapped[:, 3].reshape((len(mapped), 1))
+
+    def _compute_camera_location(self) -> np.ndarray:
+        right = self.horizontal_vect
+        up = self.vertical_vect
+        normal = get_unit_normal(right, up)
+        distance = get_norm(up) / 2 / math.tan(math.radians(self.fov / 2))
+        return self.center + normal * distance
+
+    def _compute_view_matrix(self) -> np.ndarray:
+        rot_matrix = np.eye(4)
+        rot_matrix[0, :3] = normalize(self.horizontal_vect)
+        rot_matrix[1, :3] = normalize(self.vertical_vect)
+        rot_matrix[2, :3] = normalize(self.camera_location - self.center)
+
+        shift_matrix = np.eye(4)
+        shift_matrix[:3, 3] = -self.camera_location
+
+        return np.dot(rot_matrix, shift_matrix)
+
+    def _compute_proj_matrix(self, near=0.1, far=100.0) -> np.ndarray:
+        aspect = self.horizontal_dist / self.vertical_dist
+
+        f = 1.0 / np.tan(np.radians(self.fov) / 2.0)
+        return np.array([
+            [f / aspect, 0, 0, 0],
+            [0, f, 0, 0],
+            [0, 0, (far + near) / (near - far), 2 * far * near / (near - far)],
+            [0, 0, -1, 0]
+        ])
```

### Comparing `janim-1.0.4/janim/cli.py` & `janim-1.1.0/janim/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,222 +1,225 @@
-import importlib.machinery
-import inspect
-import os
-import platform
-import subprocess as sp
-import time
-from argparse import Namespace
-
-from janim.anims.timeline import Timeline
-from janim.exception import (EXITCODE_MODULE_NOT_FOUND, EXITCODE_NOT_FILE,
-                             ExitException)
-from janim.logger import log
-from janim.utils.config import default_config
-
-
-def run(args: Namespace) -> None:
-    module = get_module(args.filepath)
-    if module is None:
-        return
-    modify_default_config(args)
-
-    timelines = extract_timelines_from_module(args, module)
-    if not timelines:
-        return
-
-    from janim.gui.anim_viewer import AnimViewer
-
-    auto_play = len(timelines) == 1
-
-    from PySide6.QtCore import QPoint, QTimer
-
-    from janim.gui.application import Application
-
-    app = Application()
-
-    log.info('======')
-
-    widgets: list[AnimViewer] = []
-    for timeline in timelines:
-        viewer = AnimViewer(timeline().build(), auto_play, args.interact)
-        widgets.append(viewer)
-
-    log.info('======')
-    log.info('Constructing window')
-
-    t = time.time()
-
-    for i, widget in enumerate(widgets):
-        if i != 0:
-            widget.move(widgets[i - 1].pos() + QPoint(24, 24))
-        widget.show()
-
-    QTimer.singleShot(200, widgets[-1].activateWindow)
-
-    log.info(f'Finished constructing in {time.time() - t:.2f} s')
-    log.info('======')
-
-    app.exec()
-
-
-def write(args: Namespace) -> None:
-    module = get_module(args.filepath)
-    if module is None:
-        return
-    modify_default_config(args)
-
-    timelines = extract_timelines_from_module(args, module)
-    if not timelines:
-        return
-
-    from janim.render.writer import AudioWriter, VideoWriter
-
-    log.info('======')
-
-    built = [timeline().build() for timeline in timelines]
-
-    log.info('======')
-
-    both = not args.video and not args.audio
-
-    log.info('======')
-
-    for anim in built:
-        name = anim.timeline.__class__.__name__
-        relative_path = os.path.dirname(inspect.getfile(anim.timeline.__class__))
-
-        output_dir = os.path.normpath(anim.cfg.formated_output_dir(relative_path))
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-
-        if both or args.video:
-            log.info(f'fps={anim.cfg.fps}')
-            log.info(f'resolution="{anim.cfg.pixel_width}x{anim.cfg.pixel_height}"')
-            log.info(f'format="{args.format}"')
-        if both or args.audio:
-            log.info(f'audio_format="{args.audio_format}"')
-            log.info(f'audio_framerate="{anim.cfg.audio_framerate}"')
-        log.info(f'output_dir="{output_dir}"')
-
-        if both or args.video:
-            writer = VideoWriter(anim)
-            writer.write_all(
-                os.path.join(output_dir,
-                             f'{name}.{args.format}')
-            )
-            if args.open and anim is built[-1]:
-                open_file(writer.final_file_path)
-
-        if (both or args.audio) and anim.timeline.has_audio():
-            writer = AudioWriter(anim)
-            writer.write_all(
-                os.path.join(output_dir,
-                             f'{name}.{args.audio_format}')
-            )
-
-    log.info('======')
-
-
-def modify_default_config(args: Namespace) -> None:
-    if args.config:
-        for key, value in args.config:
-            dtype = type(getattr(default_config, key))
-            setattr(default_config, key, dtype(value))
-
-
-def get_module(file_name: str):
-    if not os.path.exists(file_name):
-        log.error(f'"{file_name}" 不存在')
-        raise ExitException(EXITCODE_MODULE_NOT_FOUND)
-
-    if not os.path.isfile(file_name):
-        log.error(f'"{file_name}" 不是文件')
-        raise ExitException(EXITCODE_NOT_FILE)
-
-    module_name = file_name.replace(os.sep, ".").replace(".py", "")
-    loader = importlib.machinery.SourceFileLoader(module_name, file_name)
-    module = loader.load_module()
-    return module
-
-
-def extract_timelines_from_module(args: Namespace, module) -> list[type['Timeline']]:
-    from janim.anims.timeline import Timeline
-
-    timelines = []
-    err = False
-
-    if not args.all and args.timeline_names:
-        for name in args.timeline_names:
-            try:
-                timelines.append(module.__dict__[name])
-            except KeyError:
-                log.error(f'No timeline named "{name}"')
-                err = True
-    else:
-        import inspect
-
-        classes = [
-            value
-            for value in module.__dict__.values()
-            if isinstance(value, type) and issubclass(value, Timeline) and value.__module__ == module.__name__
-        ]
-        if len(classes) <= 1:
-            return classes
-        classes.sort(key=lambda x: inspect.getsourcelines(x)[1])
-        if args.all:
-            return classes
-
-        max_digits = len(str(len(classes)))
-
-        name_to_class = {}
-        for idx, timeline_class in enumerate(classes, start=1):
-            name = timeline_class.__name__
-            print(f"{str(idx).zfill(max_digits)}: {name}")
-            name_to_class[name] = timeline_class
-
-        try:
-            user_input = input(
-                "\nThat module has multiple timelines, "
-                "which ones would you like to render?"
-                "\nTimeline Name or Number: "
-            )
-        except KeyboardInterrupt:
-            user_input = ''
-
-        for split_str in user_input.replace(' ', '').split(','):
-            if not split_str:
-                continue
-            if split_str.isnumeric():
-                idx = int(split_str) - 1
-                if 0 <= idx < len(classes):
-                    timelines.append(classes[idx])
-                else:
-                    log.error(f'Invaild number {idx + 1}')
-                    err = True
-            else:
-                try:
-                    timelines.append(name_to_class[split_str])
-                except KeyError:
-                    log.error(f'No timeline named {split_str}')
-                    err = True
-
-    return [] if err else timelines
-
-
-def open_file(file_path: str) -> None:
-    current_os = platform.system()
-    if current_os == "Windows":
-        os.startfile(file_path)
-    else:
-        commands = []
-        if current_os == "Linux":
-            commands.append("xdg-open")
-        elif current_os.startswith("CYGWIN"):
-            commands.append("cygstart")
-        else:  # Assume macOS
-            commands.append("open")
-
-        commands.append(file_path)
-
-        FNULL = open(os.devnull, 'w')
-        sp.call(commands, stdout=FNULL, stderr=sp.STDOUT)
-        FNULL.close()
+import importlib.machinery
+import inspect
+import os
+import platform
+import subprocess as sp
+import time
+from argparse import Namespace
+
+from janim.anims.timeline import Timeline
+from janim.exception import (EXITCODE_MODULE_NOT_FOUND, EXITCODE_NOT_FILE,
+                             ExitException)
+from janim.logger import log
+from janim.utils.config import default_config
+
+
+def run(args: Namespace) -> None:
+    module = get_module(args.filepath)
+    if module is None:
+        return
+    modify_default_config(args)
+
+    timelines = extract_timelines_from_module(args, module)
+    if not timelines:
+        return
+
+    from janim.gui.anim_viewer import AnimViewer
+
+    auto_play = len(timelines) == 1
+
+    from PySide6.QtCore import QPoint, QTimer
+
+    from janim.gui.application import Application
+
+    app = Application()
+
+    log.info('======')
+
+    widgets: list[AnimViewer] = []
+    for timeline in timelines:
+        viewer = AnimViewer(timeline().build(), auto_play, args.interact)
+        widgets.append(viewer)
+
+    log.info('======')
+    log.info('Constructing window')
+
+    t = time.time()
+
+    for i, widget in enumerate(widgets):
+        if i != 0:
+            widget.move(widgets[i - 1].pos() + QPoint(24, 24))
+        widget.show()
+
+    QTimer.singleShot(200, widgets[-1].activateWindow)
+
+    log.info(f'Finished constructing in {time.time() - t:.2f} s')
+    log.info('======')
+
+    app.exec()
+
+
+def write(args: Namespace) -> None:
+    module = get_module(args.filepath)
+    if module is None:
+        return
+    modify_default_config(args)
+
+    timelines = extract_timelines_from_module(args, module)
+    if not timelines:
+        return
+
+    from janim.render.writer import AudioWriter, VideoWriter
+
+    log.info('======')
+
+    built = [timeline().build() for timeline in timelines]
+
+    log.info('======')
+
+    both = not args.video and not args.audio
+
+    log.info('======')
+
+    for anim in built:
+        name = anim.timeline.__class__.__name__
+        relative_path = os.path.dirname(inspect.getfile(anim.timeline.__class__))
+
+        output_dir = os.path.normpath(anim.cfg.formated_output_dir(relative_path))
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+
+        writes_video = both or args.video
+        writes_audio = (both or args.audio) and anim.timeline.has_audio()
+
+        if writes_video:
+            log.info(f'fps={anim.cfg.fps}')
+            log.info(f'resolution="{anim.cfg.pixel_width}x{anim.cfg.pixel_height}"')
+            log.info(f'format="{args.format}"')
+        if writes_audio:
+            log.info(f'audio_format="{args.audio_format}"')
+            log.info(f'audio_framerate="{anim.cfg.audio_framerate}"')
+        log.info(f'output_dir="{output_dir}"')
+
+        if writes_video:
+            writer = VideoWriter(anim)
+            writer.write_all(
+                os.path.join(output_dir,
+                             f'{name}.{args.format}')
+            )
+            if args.open and anim is built[-1]:
+                open_file(writer.final_file_path)
+
+        if writes_audio:
+            writer = AudioWriter(anim)
+            writer.write_all(
+                os.path.join(output_dir,
+                             f'{name}.{args.audio_format}')
+            )
+
+    log.info('======')
+
+
+def modify_default_config(args: Namespace) -> None:
+    if args.config:
+        for key, value in args.config:
+            dtype = type(getattr(default_config, key))
+            setattr(default_config, key, dtype(value))
+
+
+def get_module(file_name: str):
+    if not os.path.exists(file_name):
+        log.error(f'"{file_name}" 不存在')
+        raise ExitException(EXITCODE_MODULE_NOT_FOUND)
+
+    if not os.path.isfile(file_name):
+        log.error(f'"{file_name}" 不是文件')
+        raise ExitException(EXITCODE_NOT_FILE)
+
+    module_name = file_name.replace(os.sep, ".").replace(".py", "")
+    loader = importlib.machinery.SourceFileLoader(module_name, file_name)
+    module = loader.load_module()
+    return module
+
+
+def extract_timelines_from_module(args: Namespace, module) -> list[type['Timeline']]:
+    from janim.anims.timeline import Timeline
+
+    timelines = []
+    err = False
+
+    if not args.all and args.timeline_names:
+        for name in args.timeline_names:
+            try:
+                timelines.append(module.__dict__[name])
+            except KeyError:
+                log.error(f'No timeline named "{name}"')
+                err = True
+    else:
+        import inspect
+
+        classes = [
+            value
+            for value in module.__dict__.values()
+            if isinstance(value, type) and issubclass(value, Timeline) and value.__module__ == module.__name__
+        ]
+        if len(classes) <= 1:
+            return classes
+        classes.sort(key=lambda x: inspect.getsourcelines(x)[1])
+        if args.all:
+            return classes
+
+        max_digits = len(str(len(classes)))
+
+        name_to_class = {}
+        for idx, timeline_class in enumerate(classes, start=1):
+            name = timeline_class.__name__
+            print(f"{str(idx).zfill(max_digits)}: {name}")
+            name_to_class[name] = timeline_class
+
+        try:
+            user_input = input(
+                "\nThat module has multiple timelines, "
+                "which ones would you like to render?"
+                "\nTimeline Name or Number: "
+            )
+        except KeyboardInterrupt:
+            user_input = ''
+
+        for split_str in user_input.replace(' ', '').split(','):
+            if not split_str:
+                continue
+            if split_str.isnumeric():
+                idx = int(split_str) - 1
+                if 0 <= idx < len(classes):
+                    timelines.append(classes[idx])
+                else:
+                    log.error(f'Invaild number {idx + 1}')
+                    err = True
+            else:
+                try:
+                    timelines.append(name_to_class[split_str])
+                except KeyError:
+                    log.error(f'No timeline named {split_str}')
+                    err = True
+
+    return [] if err else timelines
+
+
+def open_file(file_path: str) -> None:
+    current_os = platform.system()
+    if current_os == "Windows":
+        os.startfile(file_path)
+    else:
+        commands = []
+        if current_os == "Linux":
+            commands.append("xdg-open")
+        elif current_os.startswith("CYGWIN"):
+            commands.append("cygstart")
+        else:  # Assume macOS
+            commands.append("open")
+
+        commands.append(file_path)
+
+        FNULL = open(os.devnull, 'w')
+        sp.call(commands, stdout=FNULL, stderr=sp.STDOUT)
+        FNULL.close()
```

### Comparing `janim-1.0.4/janim/components/component.py` & `janim-1.1.0/janim/components/component.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-from __future__ import annotations
-
-import copy
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Generator, Self, overload
-
-import janim.utils.refresh as refresh
-from janim.exception import CmptGroupLookupError
-from janim.utils.data import AlignedData
-
-if TYPE_CHECKING:   # pragma: no cover
-    from janim.items.item import Item
-
-
-class _CmptMeta(type):
-    def __new__(
-        cls: type,
-        name: str,
-        bases: tuple[type, ...],
-        attrdict: dict,
-        *,
-        impl=False,     # 若 impl=True，则会跳过下面的检查
-    ):
-        if not impl:
-            for key in ('copy', 'become', 'not_changed'):
-                if not callable(attrdict.get(key, None)):
-                    raise AttributeError(f'Component 的每一个子类都必须继承并实现 `{key}` 方法，而 {name} 没有')
-        return super().__new__(cls, name, bases, attrdict)
-
-
-class Component[ItemT](refresh.Refreshable, metaclass=_CmptMeta):
-    @dataclass
-    class BindInfo:
-        '''
-        对组件定义信息的封装
-
-        - ``decl_cls``: 以 ``xxx = CmptInfo(...)`` 的形式被声明在哪个类中；
-          如果一个类及其父类都有 ``xxx = CmptInfo(...)`` ，那么 ``decl_cls`` 是父类
-        - ``at_item``: 这个组件对象是属于哪个物件对象的
-        - ``key``: 这个组件对象的变量名
-
-        例：
-
-        .. code-block:: python
-
-            class MyCmpt(Component): ...
-
-            class MyItem(Item):
-                cmpt1 = CmptInfo(MyCmpt[Self])
-                cmpt2 = CmptInfo(MyCmpt[Self])
-
-            class MyItem2(MyItem):
-                cmpt3 = CmptInfo(MyCmpt[Self])
-
-            item = MyItem()
-
-            # item.cmpt1.bind_info 与 BindInfo(MyItem, item, 'cmpt1') 一致
-            # item.cmpt2.bind_info 与 BindInfo(MyItem, item, 'cmpt2') 一致
-
-            item2 = MyItem2()
-
-            # item2.cmpt1.bind_info 与 BindInfo(MyItem, item2, 'cmpt1') 一致
-            # item2.cmpt3.bind_info 与 BindInfo(MyItem2, item2, 'cmpt3') 一致
-        '''
-        decl_cls: type[Item]
-        at_item: Item
-        key: str
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.bind: Component.BindInfo | None = None
-
-    def init_bind(self, bind: BindInfo) -> None:
-        '''
-        用于 ``Item._init_components``
-
-        子类可以继承该函数，进行与所在物件相关的处理
-        '''
-        self.bind = bind
-
-    def fallback_check(self) -> bool:
-        return self.bind is not None and self.bind.at_item.stored
-
-    def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
-        '''
-        详见： :meth:`~.Item.broadcast_refresh_of_component`
-        '''
-        super().mark_refresh(func)
-
-        if self.bind is not None:
-            self.bind.at_item.broadcast_refresh_of_component(
-                self,
-                func,
-                recurse_up=recurse_up,
-                recurse_down=recurse_down
-            )
-
-    def copy(self) -> Self:
-        cmpt_copy = copy.copy(self)
-        # cmpt_copy.bind = None
-        cmpt_copy.reset_refresh()
-        return cmpt_copy
-
-    def become(self, other) -> Self: ...
-
-    def not_changed(self, other) -> bool: ...
-
-    def get_same_cmpt(self, item: Item) -> Self:
-        return self.get_same_cmpt_if_exists(item) or getattr(item.astype(self.bind.decl_cls), self.bind.key)
-
-    def get_same_cmpt_without_mock(self, item: Item) -> Self | None:
-        return item.components.get(self.bind.key, None)
-
-    def get_same_cmpt_if_exists(self, item: Item) -> Self | None:
-        cmpt = item.components.get(self.bind.key, None)
-        if cmpt is not None:
-            return cmpt
-
-        return item._astype_mock_cmpt.get(self.bind.key, None)
-
-    def walk_same_cmpt_of_self_and_descendants_without_mock(
-        self,
-        root_only: bool = False,
-        *,
-        timed: bool = False
-    ) -> Generator[Self, None, None]:
-        yield self
-        if root_only or self.bind is None:
-            return
-
-        item = self.bind.at_item
-        walk = None
-        if not item.stored:
-            walk = item.walk_descendants(self.bind.decl_cls)
-        elif timed:
-            walk = item._walk_lst(self.bind.decl_cls, item._current_family(up=False))
-
-        if walk is not None:
-            for item in walk:
-                cmpt = self.get_same_cmpt_without_mock(item)
-                if cmpt is None:
-                    continue
-                yield cmpt
-
-    @property
-    def r(self) -> ItemT:
-        '''
-        所位于的物件，便于链式调用同物件下其它的组件
-        '''
-        return self.bind.at_item
-
-
-class CmptInfo[T]:
-    '''
-    在类中定义组件需要使用该类
-
-    例：
-
-    .. code-block:: python
-
-        class MyItem(Item):
-            # Wrong!
-            # cmpt1 = MyCmpt()
-
-            # Right
-            cmpt1 = CmptInfo(MyCmpt[Self])
-
-            # Wrong!
-            # cmpt2 = MyCmptWithArgs(1)
-
-            # Right
-            cmpt2 = CmptInfo(MyCmptWithArgs[Self], 1)
-    '''
-    def __init__(self, cls: type[T], *args, **kwargs):
-        self.__doc__ = ""
-        self.cls = getattr(cls, '__origin__', cls)
-        self.args = args
-        self.kwargs = kwargs
-
-    def create(self) -> Component:
-        return self.cls(*self.args, **self.kwargs)
-
-    # 方便代码补全，没有实际意义
-    @overload
-    def __get__(self, obj: None, owner) -> Self: ...
-    @overload
-    def __get__(self, obj: object, owner) -> T: ...
-
-    def __get__(self, obj, owner):
-        return self
-
-
-class _CmptGroup(Component):
-    def __init__(self, cmpt_info_list: list[CmptInfo], **kwargs):
-        super().__init__(**kwargs)
-        self.cmpt_info_list = cmpt_info_list
-
-    def init_bind(self, bind: Component.BindInfo) -> None:
-        super().init_bind(bind)
-        self._find_objects()
-
-    def copy(self, *, new_cmpts: dict[str, Component]) -> Self:
-        cmpt_copy = super().copy()
-        cmpt_copy.objects = {
-            key: new_cmpts[key]
-            for key in cmpt_copy.objects.keys()
-        }
-
-        return cmpt_copy
-
-    def become(self, other) -> Self:    # pragma: no cover
-        return self
-
-    def not_changed(self, other: _CmptGroup) -> bool:
-        for key, obj in self.objects.items():
-            if not obj.not_changed(other.objects[key]):
-                return False
-
-        return True
-
-    @classmethod
-    def align(cls, cmpt1: _CmptGroup, cmpt2: _CmptGroup, aligned: AlignedData[Item]):
-        cmpt1_copy = cmpt1.copy(new_cmpts=aligned.data1.components)
-        cmpt2_copy = cmpt2.copy(new_cmpts=aligned.data2.components)
-        cmpt_union = cmpt1.copy(new_cmpts=aligned.union.components)
-        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt_union)
-
-    def _find_objects(self) -> None:
-        self.objects: dict[str, Component] = {}
-
-        for cmpt_info in self.cmpt_info_list:
-            key = self._find_key(cmpt_info)
-            self.objects[key] = getattr(self.bind.at_item, key)
-
-    def _find_key(self, cmpt_info: CmptInfo) -> str:
-        from janim.items.item import CLS_CMPTINFO_NAME
-
-        for key, val in self.bind.decl_cls.__dict__.get(CLS_CMPTINFO_NAME, {}).items():
-            if val is cmpt_info:
-                return key
-
-        raise CmptGroupLookupError('CmptGroup 必须要与传入的内容在同一个类的定义中')
-
-    def __getattr__(self, name: str):
-        if name == 'objects':
-            raise AttributeError()
-
-        objects = []
-        methods = []
-
-        for obj in self.objects.values():
-            if not hasattr(obj, name):
-                continue
-
-            attr = getattr(obj, name)
-            if not callable(attr):
-                continue
-
-            objects.append(obj)
-            methods.append(attr)
-
-        if not methods:
-            cmpt_str = ', '.join(cmpt.__class__.__name__ for cmpt in self.objects)
-            raise AttributeError(f'({cmpt_str}) 中没有组件有叫作 {name} 的方法')
-
-        def wrapper(*args, **kwargs):
-            ret = [
-                method(*args, **kwargs)
-                for method in methods
-            ]
-
-            return self if all(a is b for a, b in zip(ret, objects)) else ret
-
-        return wrapper
-
-
-def CmptGroup[T](*cmpt_info_list: CmptInfo[T]) -> CmptInfo[T]:
-    '''
-    用于将多个组件打包，使得可以同时调用
-
-    例：
-
-    .. code-block:: python
-
-        class MyItem(Item):
-            stroke = CmptInfo(Cmpt_Rgbas[Self])
-            fill = CmptInfo(Cmpt_Rgbas[Self])
-            color = CmptGroup(stroke, fill)
-
-        item = MyItem()
-        item.stroke.set(...)    # 只有 stroke 的被调用 | Only the method of stroke be called
-        item.color.set(...)     # stroke 和 fill 的都被调用了 | the methods of stroke and fill are both called
-    '''
-    return CmptInfo(_CmptGroup, cmpt_info_list)
+from __future__ import annotations
+
+import copy
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Callable, Generator, Self, overload
+
+import janim.utils.refresh as refresh
+from janim.exception import CmptGroupLookupError
+from janim.utils.data import AlignedData
+
+if TYPE_CHECKING:   # pragma: no cover
+    from janim.items.item import Item
+
+
+class _CmptMeta(type):
+    def __new__(
+        cls: type,
+        name: str,
+        bases: tuple[type, ...],
+        attrdict: dict,
+        *,
+        impl=False,     # 若 impl=True，则会跳过下面的检查
+    ):
+        if not impl:
+            for key in ('copy', 'become', 'not_changed'):
+                if not callable(attrdict.get(key, None)):
+                    raise AttributeError(f'Component 的每一个子类都必须继承并实现 `{key}` 方法，而 {name} 没有')
+        return super().__new__(cls, name, bases, attrdict)
+
+
+class Component[ItemT](refresh.Refreshable, metaclass=_CmptMeta):
+    @dataclass
+    class BindInfo:
+        '''
+        对组件定义信息的封装
+
+        - ``decl_cls``: 以 ``xxx = CmptInfo(...)`` 的形式被声明在哪个类中；
+          如果一个类及其父类都有 ``xxx = CmptInfo(...)`` ，那么 ``decl_cls`` 是父类
+        - ``at_item``: 这个组件对象是属于哪个物件对象的
+        - ``key``: 这个组件对象的变量名
+
+        例：
+
+        .. code-block:: python
+
+            class MyCmpt(Component): ...
+
+            class MyItem(Item):
+                cmpt1 = CmptInfo(MyCmpt[Self])
+                cmpt2 = CmptInfo(MyCmpt[Self])
+
+            class MyItem2(MyItem):
+                cmpt3 = CmptInfo(MyCmpt[Self])
+
+            item = MyItem()
+
+            # item.cmpt1.bind_info 与 BindInfo(MyItem, item, 'cmpt1') 一致
+            # item.cmpt2.bind_info 与 BindInfo(MyItem, item, 'cmpt2') 一致
+
+            item2 = MyItem2()
+
+            # item2.cmpt1.bind_info 与 BindInfo(MyItem, item2, 'cmpt1') 一致
+            # item2.cmpt3.bind_info 与 BindInfo(MyItem2, item2, 'cmpt3') 一致
+        '''
+        decl_cls: type[Item]
+        at_item: Item
+        key: str
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.bind: Component.BindInfo | None = None
+
+    def init_bind(self, bind: BindInfo) -> None:
+        '''
+        用于 ``Item._init_components``
+
+        子类可以继承该函数，进行与所在物件相关的处理
+        '''
+        self.bind = bind
+
+    def fallback_check(self) -> bool:
+        return self.bind is not None and self.bind.at_item.stored
+
+    def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
+        '''
+        详见： :meth:`~.Item.broadcast_refresh_of_component`
+        '''
+        super().mark_refresh(func)
+
+        if self.bind is not None:
+            self.bind.at_item.broadcast_refresh_of_component(
+                self,
+                func,
+                recurse_up=recurse_up,
+                recurse_down=recurse_down
+            )
+
+    def copy(self) -> Self:
+        cmpt_copy = copy.copy(self)
+        # cmpt_copy.bind = None
+        cmpt_copy.reset_refresh()
+        return cmpt_copy
+
+    def become(self, other) -> Self: ...
+
+    def not_changed(self, other) -> bool: ...
+
+    def get_same_cmpt(self, item: Item) -> Self:
+        return self.get_same_cmpt_if_exists(item) or getattr(item.astype(self.bind.decl_cls), self.bind.key)
+
+    def get_same_cmpt_without_mock(self, item: Item) -> Self | None:
+        return item.components.get(self.bind.key, None)
+
+    def get_same_cmpt_if_exists(self, item: Item) -> Self | None:
+        cmpt = item.components.get(self.bind.key, None)
+        if cmpt is not None:
+            return cmpt
+
+        return item._astype_mock_cmpt.get(self.bind.key, None)
+
+    def walk_same_cmpt_of_self_and_descendants_without_mock(
+        self,
+        root_only: bool = False,
+        *,
+        timed: bool = False
+    ) -> Generator[Self, None, None]:
+        yield self
+        if root_only or self.bind is None:
+            return
+
+        item = self.bind.at_item
+        walk = None
+        if not item.stored:
+            walk = item.walk_descendants(self.bind.decl_cls)
+        elif timed:
+            walk = item._walk_lst(self.bind.decl_cls, item._current_family(up=False))
+
+        if walk is not None:
+            for item in walk:
+                cmpt = self.get_same_cmpt_without_mock(item)
+                if cmpt is None:
+                    continue
+                yield cmpt
+
+    @property
+    def r(self) -> ItemT:
+        '''
+        所位于的物件，便于链式调用同物件下其它的组件
+        '''
+        return self.bind.at_item
+
+
+class CmptInfo[T]:
+    '''
+    在类中定义组件需要使用该类
+
+    例：
+
+    .. code-block:: python
+
+        class MyItem(Item):
+            # Wrong!
+            # cmpt1 = MyCmpt()
+
+            # Right
+            cmpt1 = CmptInfo(MyCmpt[Self])
+
+            # Wrong!
+            # cmpt2 = MyCmptWithArgs(1)
+
+            # Right
+            cmpt2 = CmptInfo(MyCmptWithArgs[Self], 1)
+    '''
+    def __init__(self, cls: type[T], *args, **kwargs):
+        self.__doc__ = ""
+        self.cls = getattr(cls, '__origin__', cls)
+        self.args = args
+        self.kwargs = kwargs
+
+    def create(self) -> Component:
+        return self.cls(*self.args, **self.kwargs)
+
+    # 方便代码补全，没有实际意义
+    @overload
+    def __get__(self, obj: None, owner) -> Self: ...
+    @overload
+    def __get__(self, obj: object, owner) -> T: ...
+
+    def __get__(self, obj, owner):
+        return self
+
+
+class _CmptGroup(Component):
+    def __init__(self, cmpt_info_list: list[CmptInfo], **kwargs):
+        super().__init__(**kwargs)
+        self.cmpt_info_list = cmpt_info_list
+
+    def init_bind(self, bind: Component.BindInfo) -> None:
+        super().init_bind(bind)
+        self._find_objects()
+
+    def copy(self, *, new_cmpts: dict[str, Component]) -> Self:
+        cmpt_copy = super().copy()
+        cmpt_copy.objects = {
+            key: new_cmpts[key]
+            for key in cmpt_copy.objects.keys()
+        }
+
+        return cmpt_copy
+
+    def become(self, other) -> Self:    # pragma: no cover
+        return self
+
+    def not_changed(self, other: _CmptGroup) -> bool:
+        for key, obj in self.objects.items():
+            if not obj.not_changed(other.objects[key]):
+                return False
+
+        return True
+
+    @classmethod
+    def align(cls, cmpt1: _CmptGroup, cmpt2: _CmptGroup, aligned: AlignedData[Item]):
+        cmpt1_copy = cmpt1.copy(new_cmpts=aligned.data1.components)
+        cmpt2_copy = cmpt2.copy(new_cmpts=aligned.data2.components)
+        cmpt_union = cmpt1.copy(new_cmpts=aligned.union.components)
+        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt_union)
+
+    def _find_objects(self) -> None:
+        self.objects: dict[str, Component] = {}
+
+        for cmpt_info in self.cmpt_info_list:
+            key = self._find_key(cmpt_info)
+            self.objects[key] = getattr(self.bind.at_item, key)
+
+    def _find_key(self, cmpt_info: CmptInfo) -> str:
+        from janim.items.item import CLS_CMPTINFO_NAME
+
+        for key, val in self.bind.decl_cls.__dict__.get(CLS_CMPTINFO_NAME, {}).items():
+            if val is cmpt_info:
+                return key
+
+        raise CmptGroupLookupError('CmptGroup 必须要与传入的内容在同一个类的定义中')
+
+    def __getattr__(self, name: str):
+        if name == 'objects':
+            raise AttributeError()
+
+        objects = []
+        methods = []
+
+        for obj in self.objects.values():
+            if not hasattr(obj, name):
+                continue
+
+            attr = getattr(obj, name)
+            if not callable(attr):
+                continue
+
+            objects.append(obj)
+            methods.append(attr)
+
+        if not methods:
+            cmpt_str = ', '.join(cmpt.__class__.__name__ for cmpt in self.objects)
+            raise AttributeError(f'({cmpt_str}) 中没有组件有叫作 {name} 的方法')
+
+        def wrapper(*args, **kwargs):
+            ret = [
+                method(*args, **kwargs)
+                for method in methods
+            ]
+
+            return self if all(a is b for a, b in zip(ret, objects)) else ret
+
+        return wrapper
+
+
+def CmptGroup[T](*cmpt_info_list: CmptInfo[T]) -> CmptInfo[T]:
+    '''
+    用于将多个组件打包，使得可以同时调用
+
+    例：
+
+    .. code-block:: python
+
+        class MyItem(Item):
+            stroke = CmptInfo(Cmpt_Rgbas[Self])
+            fill = CmptInfo(Cmpt_Rgbas[Self])
+            color = CmptGroup(stroke, fill)
+
+        item = MyItem()
+        item.stroke.set(...)    # 只有 stroke 的被调用 | Only the method of stroke be called
+        item.color.set(...)     # stroke 和 fill 的都被调用了 | the methods of stroke and fill are both called
+    '''
+    return CmptInfo(_CmptGroup, cmpt_info_list)
```

### Comparing `janim-1.0.4/janim/components/data.py` & `janim-1.1.0/janim/components/data.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from __future__ import annotations
-
-from typing import Callable, Self
-
-from janim.components.component import Component
-from janim.utils.data import AlignedData
-
-type CopyFn[T] = Callable[[T], T]
-type MaybeSameFn[T] = Callable[[T, T], bool]
-type InterpolateFn[T] = Callable[[T, T, float], T]
-
-
-class Cmpt_Data[ItemT, T](Component[ItemT]):
-    '''
-    详见 :class:`~.ValueTracker`
-    '''
-    def __init__(self):
-        self.copy_func: CopyFn[T] = None
-        self.maybe_same_func: MaybeSameFn[T] = None
-        self.interpolate_func: InterpolateFn[T] = None
-
-    def copy(self) -> Self:
-        cmpt_copy = super().copy()
-
-        assert self.copy_func is not None
-        cmpt_copy.set(self.copy_func(self.value))
-
-        return cmpt_copy
-
-    def become(self, other: Cmpt_Data) -> Self:
-        self.set(other.copy_func(other.value))
-        return self
-
-    def not_changed(self, other: Cmpt_Data) -> bool:
-        assert self.maybe_same_func is not None
-        return self.maybe_same_func(self.value, other.value)
-
-    @classmethod
-    def align_for_interpolate(cls, cmpt1: Cmpt_Data, cmpt2: Cmpt_Data) -> AlignedData[Self]:
-        cmpt1_copy = cmpt1.copy()
-        cmpt2_copy = cmpt2.copy()
-        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
-
-    def interpolate(self, cmpt1: Cmpt_Data, cmpt2: Cmpt_Data, alpha: float, *, path_func=None) -> Self:
-        if cmpt1 == cmpt2:
-            return
-
-        self.set(self.interpolate_func(cmpt1.value, cmpt2.value, alpha))
-        return self
-
-    def set(self, value: T) -> Self:
-        '''设置当前数据'''
-        self.value = value
-        return self
-
-    def increment(self, value: T) -> Self:
-        '''将值增加 ``value``'''
-        self.value += value
-        return self
-
-    def get(self) -> T:
-        '''得到当前数据'''
-        return self.value
-
-    def set_func(
-        self,
-        copy_func: CopyFn[T] | None = None,
-        maybe_same_func: MaybeSameFn[T] | None = None,
-        interpolate_func: InterpolateFn[T] | None = None
-    ) -> Self:
-        if copy_func is not None:
-            self.copy_func = copy_func
-        if maybe_same_func is not None:
-            self.maybe_same_func = maybe_same_func
-        if interpolate_func is not None:
-            self.interpolate_func = interpolate_func
-        return self
+from __future__ import annotations
+
+from typing import Callable, Self
+
+from janim.components.component import Component
+from janim.utils.data import AlignedData
+
+type CopyFn[T] = Callable[[T], T]
+type MaybeSameFn[T] = Callable[[T, T], bool]
+type InterpolateFn[T] = Callable[[T, T, float], T]
+
+
+class Cmpt_Data[ItemT, T](Component[ItemT]):
+    '''
+    详见 :class:`~.ValueTracker`
+    '''
+    def __init__(self):
+        self.copy_func: CopyFn[T] = None
+        self.maybe_same_func: MaybeSameFn[T] = None
+        self.interpolate_func: InterpolateFn[T] = None
+
+    def copy(self) -> Self:
+        cmpt_copy = super().copy()
+
+        assert self.copy_func is not None
+        cmpt_copy.set(self.copy_func(self.value))
+
+        return cmpt_copy
+
+    def become(self, other: Cmpt_Data) -> Self:
+        self.set(other.copy_func(other.value))
+        return self
+
+    def not_changed(self, other: Cmpt_Data) -> bool:
+        assert self.maybe_same_func is not None
+        return self.maybe_same_func(self.value, other.value)
+
+    @classmethod
+    def align_for_interpolate(cls, cmpt1: Cmpt_Data, cmpt2: Cmpt_Data) -> AlignedData[Self]:
+        cmpt1_copy = cmpt1.copy()
+        cmpt2_copy = cmpt2.copy()
+        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
+
+    def interpolate(self, cmpt1: Cmpt_Data, cmpt2: Cmpt_Data, alpha: float, *, path_func=None) -> Self:
+        if cmpt1 == cmpt2:
+            return
+
+        self.set(self.interpolate_func(cmpt1.value, cmpt2.value, alpha))
+        return self
+
+    def set(self, value: T) -> Self:
+        '''设置当前数据'''
+        self.value = value
+        return self
+
+    def increment(self, value: T) -> Self:
+        '''将值增加 ``value``'''
+        self.value += value
+        return self
+
+    def get(self) -> T:
+        '''得到当前数据'''
+        return self.value
+
+    def set_func(
+        self,
+        copy_func: CopyFn[T] | None = None,
+        maybe_same_func: MaybeSameFn[T] | None = None,
+        interpolate_func: InterpolateFn[T] | None = None
+    ) -> Self:
+        if copy_func is not None:
+            self.copy_func = copy_func
+        if maybe_same_func is not None:
+            self.maybe_same_func = maybe_same_func
+        if interpolate_func is not None:
+            self.interpolate_func = interpolate_func
+        return self
```

### Comparing `janim-1.0.4/janim/components/depth.py` & `janim-1.1.0/janim/components/depth.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from __future__ import annotations
-
-from collections import defaultdict
-from typing import Self
-
-from janim.components.component import Component
-
-
-class Cmpt_Depth[ItemT](Component[ItemT]):
-    '''深度组件
-
-    - 如果某个对象的深度值更小，那么它在 ``>`` 和 ``<`` 的判断中也就更小
-    - 如果两个对象的深度值相同，那么后创建的对象在 ``>`` 和 ``<`` 的判断中更小
-
-    被用于绘制时，也就是说：
-
-    - 深度大的会被深度小的遮盖
-    - 深度一样时，先创建的会被后创建的遮盖
-
-    例：
-
-    .. code-block:: python
-
-        d1 = Depth(0)
-        d2 = Depth(2)
-        d3 = Depth(2)
-
-        print(d1 < d3)  # True
-        print(d2 < d3)  # False
-        print(d2 > d3)  # True
-
-    上面这个例子的绘制顺序（从最早被绘制的到最迟被绘制的）：
-
-    d2、d3、d1
-
-    也就是 d3 会盖住 d2；d1 会盖住 d2 和 d3
-    '''
-    _counter: defaultdict[float, int] = defaultdict(int)
-
-    def __init__(self, value: float, order: int | None = None):
-        super().__init__()
-        self.set(value, order=order)
-
-    def copy(self) -> Self:
-        # Component.copy 中的 copy.copy(self) 已将 _value 和 _order 拷贝
-        return super().copy()
-
-    def become(self, other: Cmpt_Depth) -> Self:
-        self.set(*other.get_raw())
-        return self
-
-    def not_changed(self, other: Cmpt_Depth) -> bool:
-        return self._depth == other._depth and self._order == other._order
-
-    def __lt__(self, other: Cmpt_Depth) -> bool:
-        if self._depth != other._depth:
-            return self._depth < other._depth
-        return self._order < other._order
-
-    def set(self, value: float, order: int | None = None) -> Self:
-        '''
-        设置物件的深度
-        '''
-        self._depth = value
-        if order is None:
-            order = self._counter[value]
-            self._counter[value] -= 1
-        self._order = order
-        return self
-
-    def get(self) -> float:
-        return self._depth
-
-    def get_raw(self) -> tuple[float, int]:
-        '''
-        返回元组 ``(depth, order)``
-        '''
-        return (self._depth, self._order)
-
-    def arrange(self, depth: float | None = None) -> Self:
-        '''
-        将子物件排序深度
-        '''
-        if depth is None:
-            depth = self._depth
-
-        self.set(depth)
-
-        if self.bind is not None:
-            for item in self.bind.at_item.descendants():
-                item.depth.set(depth)
+from __future__ import annotations
+
+from collections import defaultdict
+from typing import Self
+
+from janim.components.component import Component
+
+
+class Cmpt_Depth[ItemT](Component[ItemT]):
+    '''深度组件
+
+    - 如果某个对象的深度值更小，那么它在 ``>`` 和 ``<`` 的判断中也就更小
+    - 如果两个对象的深度值相同，那么后创建的对象在 ``>`` 和 ``<`` 的判断中更小
+
+    被用于绘制时，也就是说：
+
+    - 深度大的会被深度小的遮盖
+    - 深度一样时，先创建的会被后创建的遮盖
+
+    例：
+
+    .. code-block:: python
+
+        d1 = Depth(0)
+        d2 = Depth(2)
+        d3 = Depth(2)
+
+        print(d1 < d3)  # True
+        print(d2 < d3)  # False
+        print(d2 > d3)  # True
+
+    上面这个例子的绘制顺序（从最早被绘制的到最迟被绘制的）：
+
+    d2、d3、d1
+
+    也就是 d3 会盖住 d2；d1 会盖住 d2 和 d3
+    '''
+    _counter: defaultdict[float, int] = defaultdict(int)
+
+    def __init__(self, value: float, order: int | None = None):
+        super().__init__()
+        self.set(value, order=order)
+
+    def copy(self) -> Self:
+        # Component.copy 中的 copy.copy(self) 已将 _value 和 _order 拷贝
+        return super().copy()
+
+    def become(self, other: Cmpt_Depth) -> Self:
+        self.set(*other.get_raw())
+        return self
+
+    def not_changed(self, other: Cmpt_Depth) -> bool:
+        return self._depth == other._depth and self._order == other._order
+
+    def __lt__(self, other: Cmpt_Depth) -> bool:
+        if self._depth != other._depth:
+            return self._depth < other._depth
+        return self._order < other._order
+
+    def set(self, value: float, order: int | None = None) -> Self:
+        '''
+        设置物件的深度
+        '''
+        self._depth = value
+        if order is None:
+            order = self._counter[value]
+            self._counter[value] -= 1
+        self._order = order
+        return self
+
+    def get(self) -> float:
+        return self._depth
+
+    def get_raw(self) -> tuple[float, int]:
+        '''
+        返回元组 ``(depth, order)``
+        '''
+        return (self._depth, self._order)
+
+    def arrange(self, depth: float | None = None) -> Self:
+        '''
+        将子物件排序深度
+        '''
+        if depth is None:
+            depth = self._depth
+
+        self.set(depth)
+
+        if self.bind is not None:
+            for item in self.bind.at_item.descendants():
+                item.depth.set(depth)
```

### Comparing `janim-1.0.4/janim/components/image.py` & `janim-1.1.0/janim/components/image.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from __future__ import annotations
-
-from typing import Self
-
-from PIL import Image
-
-from janim.components.component import Component
-
-
-class Cmpt_Image(Component):
-    '''
-    图像组件，包含一个 PIL 图像以及 ``min_mag_filter``
-    '''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.img = None
-        self.min_mag_filter = None
-
-    def copy(self) -> Self:
-        # self.img 没必要 copy
-        # self.min_mag_filter 已通过父方法 copy.copy 复制
-        return super().copy()
-
-    def become(self, other: Cmpt_Image) -> Self:
-        self.set(other.img, other.min_mag_filter)
-        return self
-
-    def not_changed(self, other: Cmpt_Image) -> bool:
-        return id(self.img) == id(other.img) and self.min_mag_filter == other.min_mag_filter
-
-    def set(self, img: Image.Image | None, min_mag_filter: int | None) -> Self:
-        '''
-        设置 PIL 图像
-        '''
-        if img is not None:
-            self.img = img
-        if min_mag_filter is not None:
-            self.min_mag_filter = min_mag_filter
-        return self
-
-    def get(self) -> Image.Image:
-        return self.img
-
-    def get_filter(self) -> int:
-        return self.min_mag_filter
+from __future__ import annotations
+
+from typing import Self
+
+from PIL import Image
+
+from janim.components.component import Component
+
+
+class Cmpt_Image(Component):
+    '''
+    图像组件，包含一个 PIL 图像以及 ``min_mag_filter``
+    '''
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.img = None
+        self.min_mag_filter = None
+
+    def copy(self) -> Self:
+        # self.img 没必要 copy
+        # self.min_mag_filter 已通过父方法 copy.copy 复制
+        return super().copy()
+
+    def become(self, other: Cmpt_Image) -> Self:
+        self.set(other.img, other.min_mag_filter)
+        return self
+
+    def not_changed(self, other: Cmpt_Image) -> bool:
+        return id(self.img) == id(other.img) and self.min_mag_filter == other.min_mag_filter
+
+    def set(self, img: Image.Image | None, min_mag_filter: int | None) -> Self:
+        '''
+        设置 PIL 图像
+        '''
+        if img is not None:
+            self.img = img
+        if min_mag_filter is not None:
+            self.min_mag_filter = min_mag_filter
+        return self
+
+    def get(self) -> Image.Image:
+        return self.img
+
+    def get_filter(self) -> int:
+        return self.min_mag_filter
```

### Comparing `janim-1.0.4/janim/components/radius.py` & `janim-1.1.0/janim/components/radius.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from __future__ import annotations
-
-from typing import Iterable, Self
-
-import numpy as np
-
-from janim.components.component import Component
-from janim.utils.bezier import interpolate
-from janim.utils.data import AlignedData, Array
-from janim.utils.iterables import resize_with_interpolation
-
-
-class Cmpt_Radius[ItemT](Component[ItemT]):
-    '''
-    半径组件，被用于 :class:`DotCloud` 的点半径，以及 :class:`VItem` 的轮廓线粗细
-    '''
-    def __init__(self, default_radius: float, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.default_radius = default_radius
-
-        self._radii = Array()
-        self._radii.data = np.full(1, self.default_radius)
-
-    def copy(self) -> Self:
-        cmpt_copy = super().copy()
-        cmpt_copy._radii = self._radii.copy()
-        return cmpt_copy
-
-    def become(self, other: Cmpt_Radius) -> Self:
-        self.set(other.get())
-        return self
-
-    def not_changed(self, other: Cmpt_Radius) -> bool:
-        return self._radii.is_share(other._radii)
-
-    @classmethod
-    def align_for_interpolate(cls, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius):
-        len1, len2 = len(cmpt1.get()), len(cmpt2.get())
-
-        cmpt1_copy = cmpt1.copy()
-        cmpt2_copy = cmpt2.copy()
-
-        if len1 < len2:
-            cmpt1_copy.resize(len2)
-        elif len1 > len2:
-            cmpt1_copy.resize(len1)
-
-        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
-
-    def interpolate(self, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius, alpha: float, *, path_func=None) -> None:
-        if cmpt1.not_changed(cmpt2):
-            return
-
-        self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
-
-    # region 半径数据 | Radii
-
-    def get(self) -> np.ndarray:
-        '''
-        得到半径数据
-        '''
-        return self._radii.data
-
-    def set(
-        self,
-        radius: float | Iterable[float],
-        *,
-        root_only: bool = False,
-    ) -> Self:
-        '''
-        设置半径数据
-        '''
-        if not isinstance(radius, Iterable):
-            radius = [radius]
-        radii = Array()
-        radii.data = radius
-
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            cmpt._radii.data = radii
-
-        return self
-
-    def clear(self) -> Self:
-        '''
-        将半径数据重置为默认值
-        '''
-        self.set(np.full(1, self.default_radius))
-
-    def reverse(self) -> Self:
-        self.set(self.get()[::-1])
-        return self
-
-    def resize(self, length: int) -> Self:
-        self.set(resize_with_interpolation(self.get(), max(1, length)))
-        return self
-
-    def count(self) -> int:
-        return len(self.get())
-
-    # endregion
+from __future__ import annotations
+
+from typing import Iterable, Self
+
+import numpy as np
+
+from janim.components.component import Component
+from janim.utils.bezier import interpolate
+from janim.utils.data import AlignedData, Array
+from janim.utils.iterables import resize_with_interpolation
+
+
+class Cmpt_Radius[ItemT](Component[ItemT]):
+    '''
+    半径组件，被用于 :class:`DotCloud` 的点半径，以及 :class:`VItem` 的轮廓线粗细
+    '''
+    def __init__(self, default_radius: float, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.default_radius = default_radius
+
+        self._radii = Array()
+        self._radii.data = np.full(1, self.default_radius)
+
+    def copy(self) -> Self:
+        cmpt_copy = super().copy()
+        cmpt_copy._radii = self._radii.copy()
+        return cmpt_copy
+
+    def become(self, other: Cmpt_Radius) -> Self:
+        self.set(other.get())
+        return self
+
+    def not_changed(self, other: Cmpt_Radius) -> bool:
+        return self._radii.is_share(other._radii)
+
+    @classmethod
+    def align_for_interpolate(cls, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius):
+        len1, len2 = len(cmpt1.get()), len(cmpt2.get())
+
+        cmpt1_copy = cmpt1.copy()
+        cmpt2_copy = cmpt2.copy()
+
+        if len1 < len2:
+            cmpt1_copy.resize(len2)
+        elif len1 > len2:
+            cmpt1_copy.resize(len1)
+
+        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
+
+    def interpolate(self, cmpt1: Cmpt_Radius, cmpt2: Cmpt_Radius, alpha: float, *, path_func=None) -> None:
+        if cmpt1.not_changed(cmpt2):
+            return
+
+        self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
+
+    # region 半径数据 | Radii
+
+    def get(self) -> np.ndarray:
+        '''
+        得到半径数据
+        '''
+        return self._radii.data
+
+    def set(
+        self,
+        radius: float | Iterable[float],
+        *,
+        root_only: bool = False,
+    ) -> Self:
+        '''
+        设置半径数据
+        '''
+        if not isinstance(radius, Iterable):
+            radius = [radius]
+        radii = Array()
+        radii.data = radius
+
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            cmpt._radii.data = radii
+
+        return self
+
+    def clear(self) -> Self:
+        '''
+        将半径数据重置为默认值
+        '''
+        self.set(np.full(1, self.default_radius))
+
+    def reverse(self) -> Self:
+        self.set(self.get()[::-1])
+        return self
+
+    def resize(self, length: int) -> Self:
+        self.set(resize_with_interpolation(self.get(), max(1, length)))
+        return self
+
+    def count(self) -> int:
+        return len(self.get())
+
+    # endregion
```

### Comparing `janim-1.0.4/janim/components/rgbas.py` & `janim-1.1.0/janim/components/rgbas.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from __future__ import annotations
-
-from typing import Iterable, Self
-
-import numpy as np
-from colour import Color
-
-from janim.components.component import Component
-from janim.typing import Alpha, AlphaArray, ColorArray, JAnimColor, RgbaArray
-from janim.utils.bezier import interpolate
-from janim.utils.data import AlignedData, Array
-from janim.utils.iterables import resize_with_interpolation
-
-DEFAULT_RGBAS_DATA = np.full((1, 4), 1)
-
-
-class Cmpt_Rgbas[ItemT](Component[ItemT]):
-    '''
-    颜色组件
-    '''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self._rgbas = Array()
-        self._rgbas.data = DEFAULT_RGBAS_DATA
-
-    def copy(self) -> Self:
-        cmpt_copy = super().copy()
-        cmpt_copy._rgbas = self._rgbas.copy()
-        return cmpt_copy
-
-    def become(self, other: Cmpt_Rgbas) -> Self:
-        self.set(other.get())
-        return self
-
-    def not_changed(self, other: Cmpt_Rgbas) -> bool:
-        return self._rgbas.is_share(other._rgbas)
-
-    @classmethod
-    def align_for_interpolate(cls, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas):
-        len1, len2 = len(cmpt1.get()), len(cmpt2.get())
-
-        cmpt1_copy = cmpt1.copy()
-        cmpt2_copy = cmpt2.copy()
-
-        if len1 < len2:
-            cmpt1_copy.resize(len2)
-        elif len1 > len2:
-            cmpt1_copy.resize(len1)
-
-        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
-
-    def interpolate(self, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas, alpha: float, *, path_func=None) -> None:
-        if cmpt1.not_changed(cmpt2):
-            return
-
-        self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
-
-    # region 颜色数据 | Colors
-
-    def get(self) -> np.ndarray:
-        return self._rgbas.data
-
-    @staticmethod
-    def format_rgbas(rgbas: RgbaArray) -> np.ndarray:
-        '''
-        将传入值转换为数值数组
-        '''
-        if not isinstance(rgbas, np.ndarray):
-            rgbas = np.array(rgbas)
-
-        assert rgbas.ndim == 2
-        assert rgbas.shape[1] == 4
-        return rgbas
-
-    @staticmethod
-    def format_colors(colors: ColorArray) -> np.ndarray:
-        '''
-        将 ``ColorArray`` （每个元素有可能是 字符串、``[r, g, b]`` ）
-        格式化为元素仅有 ``[r, g, b]`` 的数值数组的格式
-        '''
-        if not isinstance(colors, np.ndarray):
-            colors = np.array([
-                color
-                if isinstance(color, Iterable) and not isinstance(color, str)
-                else Color(color).rgb
-
-                for color in colors
-            ])
-
-        assert colors.ndim == 2
-        assert colors.shape[1] == 3
-        return colors
-
-    @staticmethod
-    def format_alphas(alphas: AlphaArray) -> np.ndarray:
-        '''
-        将传入值转为数值数组
-        '''
-        if not isinstance(alphas, np.ndarray):
-            alphas = np.array(alphas)
-
-        assert alphas.ndim == 1
-        return alphas
-
-    def set_rgbas(self, rgbas: RgbaArray) -> Self:
-        '''
-        直接设置 rgba 数据
-        '''
-        self._rgbas.data = rgbas
-        return self
-
-    def set(
-        self,
-        color: JAnimColor | ColorArray = None,
-        alpha: Alpha | AlphaArray = None,
-        *,
-        root_only: bool = False,
-    ) -> Self:
-        '''
-        - ``colors`` 表示传入的 ``RGB`` 颜色数据，可以是单个颜色也可以颜色数组
-          （对于单个数据，支持 ``'#FF0000'`` ``'red'`` ``[1, 0, 0.5]`` 的表示）
-        - ``alphas`` 表示传入的透明度数据，可以是单个数也可以是一个数组
-          （对于单个数据，``1`` 表示不透明，``0`` 表示完全透明）
-        - 默认情况下会将所有子物件也设置成指定的颜色，传入 ``root_only=True`` 可以只设置根物件的
-
-        特殊传参：
-
-        - 当 ``colors`` 为四分量 ``RGBA`` 颜色数据时，
-          则同时表示了 ``colors`` 和 ``alphas`` 二者，因此不能再传入 ``alphas`` 参数
-        '''
-        if color is None and alpha is None:
-            return self
-
-        def is_single_color(value: Iterable) -> bool:
-            if isinstance(value, str):
-                return True
-            if isinstance(value[0], str):
-                return False
-            return not isinstance(value[0], Iterable)
-
-        if color is not None and is_single_color(color):
-            color = [color]
-        if alpha is not None and not isinstance(alpha, Iterable):
-            alpha = [alpha]
-
-        if alpha is None and not isinstance(color[0], str) and len(color[0]) == 4:
-            rgbas = self.format_rgbas(color)
-
-            self.set_rgbas(rgbas)
-
-            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-                cmpt.set_rgbas(rgbas)
-
-        else:
-            if color is not None:
-                color = self.format_colors(color)
-            if alpha is not None:
-                alpha = self.format_alphas(alpha)
-
-            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-                cmpt_color = cmpt.get()[:, :3] if color is None else color
-                cmpt_alpha = cmpt.get()[:, 3] if alpha is None else alpha
-                length = max(len(cmpt_color), len(cmpt_alpha))
-
-                rgbas = np.hstack([
-                    resize_with_interpolation(cmpt_color.astype(float), length),
-                    resize_with_interpolation(cmpt_alpha.astype(float), length).reshape((length, 1))
-                ])
-                cmpt.set_rgbas(rgbas)
-
-        return self
-
-    def clear(self) -> Self:
-        '''
-        将颜色数据重置为默认值
-        '''
-        self.set(DEFAULT_RGBAS_DATA)
-        return self
-
-    def reverse(self) -> Self:
-        self.set_rgbas(self.get()[::-1])
-        return self
-
-    def resize(self, length: int) -> Self:
-        self.set(resize_with_interpolation(self.get(), max(1, length)))
-        return self
-
-    def count(self) -> int:
-        return len(self.get())
-
-    def apart_alpha(self, n: int) -> Self:
-        '''
-        对每一个颜色数据应用 :func:`~.apart_alpha`
-        '''
-        rgbas = self.get().copy()
-        for i in range(len(rgbas)):
-            rgbas[i, 3] = apart_alpha(rgbas[i, 3], n)
-        self.set_rgbas(rgbas)
-        return self
-
-    def fade(self, factor: float | Iterable[float], *, root_only: bool = False) -> Self:
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            rgbas = cmpt.get().copy()
-            rgbas[:, 3] *= 1 - factor
-            cmpt.set_rgbas(rgbas)
-
-        return self
-
-    # endregion
-
-
-def merge_alpha(alpha: float, n: int) -> float:
-    '''
-    计算透明度 ``alpha`` 在重叠 ``n`` 次混合后的透明度
-    '''
-    result = alpha
-    for _ in range(n - 1):
-        result = 1 - (1 - result) * (1 - alpha)
-
-    return result
-
-
-def apart_alpha(alpha: float, n: int, *, eps: float = 1e-3) -> float:
-    '''
-    将透明度分离为 ``n`` 份，使得这 ``n`` 份混合后仍然表现为原来的透明度
-
-    使得在对齐时产生的重复部分能够更好地渲染
-    '''
-    if alpha >= 1:
-        return 1
-    if alpha <= 0:
-        return 0
-
-    tpl1 = (0, 0)
-    tpl2 = (1, 1)
-
-    # REFACTOR: 有无更好的方式？
-    while tpl2[0] - tpl1[0] > eps:
-        mid_single = (tpl1[0] + tpl2[0]) / 2
-        mid_merged = merge_alpha(mid_single, n)
-        if mid_merged == alpha:
-            return mid_single
-
-        if mid_merged < alpha:
-            tpl1 = (mid_single, mid_merged)
-        else:
-            tpl2 = (mid_single, mid_merged)
-
-    return mid_single
+from __future__ import annotations
+
+from typing import Iterable, Self
+
+import numpy as np
+from colour import Color
+
+from janim.components.component import Component
+from janim.typing import Alpha, AlphaArray, ColorArray, JAnimColor, RgbaArray
+from janim.utils.bezier import interpolate
+from janim.utils.data import AlignedData, Array
+from janim.utils.iterables import resize_with_interpolation
+
+DEFAULT_RGBAS_DATA = np.full((1, 4), 1)
+
+
+class Cmpt_Rgbas[ItemT](Component[ItemT]):
+    '''
+    颜色组件
+    '''
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self._rgbas = Array()
+        self._rgbas.data = DEFAULT_RGBAS_DATA
+
+    def copy(self) -> Self:
+        cmpt_copy = super().copy()
+        cmpt_copy._rgbas = self._rgbas.copy()
+        return cmpt_copy
+
+    def become(self, other: Cmpt_Rgbas) -> Self:
+        self.set(other.get())
+        return self
+
+    def not_changed(self, other: Cmpt_Rgbas) -> bool:
+        return self._rgbas.is_share(other._rgbas)
+
+    @classmethod
+    def align_for_interpolate(cls, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas):
+        len1, len2 = len(cmpt1.get()), len(cmpt2.get())
+
+        cmpt1_copy = cmpt1.copy()
+        cmpt2_copy = cmpt2.copy()
+
+        if len1 < len2:
+            cmpt1_copy.resize(len2)
+        elif len1 > len2:
+            cmpt1_copy.resize(len1)
+
+        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
+
+    def interpolate(self, cmpt1: Cmpt_Rgbas, cmpt2: Cmpt_Rgbas, alpha: float, *, path_func=None) -> None:
+        if cmpt1.not_changed(cmpt2):
+            return
+
+        self.set(interpolate(cmpt1.get(), cmpt2.get(), alpha))
+
+    # region 颜色数据 | Colors
+
+    def get(self) -> np.ndarray:
+        return self._rgbas.data
+
+    @staticmethod
+    def format_rgbas(rgbas: RgbaArray) -> np.ndarray:
+        '''
+        将传入值转换为数值数组
+        '''
+        if not isinstance(rgbas, np.ndarray):
+            rgbas = np.array(rgbas)
+
+        assert rgbas.ndim == 2
+        assert rgbas.shape[1] == 4
+        return rgbas
+
+    @staticmethod
+    def format_colors(colors: ColorArray) -> np.ndarray:
+        '''
+        将 ``ColorArray`` （每个元素有可能是 字符串、``[r, g, b]`` ）
+        格式化为元素仅有 ``[r, g, b]`` 的数值数组的格式
+        '''
+        if not isinstance(colors, np.ndarray):
+            colors = np.array([
+                color
+                if isinstance(color, Iterable) and not isinstance(color, str)
+                else Color(color).rgb
+
+                for color in colors
+            ])
+
+        assert colors.ndim == 2
+        assert colors.shape[1] == 3
+        return colors
+
+    @staticmethod
+    def format_alphas(alphas: AlphaArray) -> np.ndarray:
+        '''
+        将传入值转为数值数组
+        '''
+        if not isinstance(alphas, np.ndarray):
+            alphas = np.array(alphas)
+
+        assert alphas.ndim == 1
+        return alphas
+
+    def set_rgbas(self, rgbas: RgbaArray) -> Self:
+        '''
+        直接设置 rgba 数据
+        '''
+        self._rgbas.data = rgbas
+        return self
+
+    def set(
+        self,
+        color: JAnimColor | ColorArray = None,
+        alpha: Alpha | AlphaArray = None,
+        *,
+        root_only: bool = False,
+    ) -> Self:
+        '''
+        - ``colors`` 表示传入的 ``RGB`` 颜色数据，可以是单个颜色也可以颜色数组
+          （对于单个数据，支持 ``'#FF0000'`` ``'red'`` ``[1, 0, 0.5]`` 的表示）
+        - ``alphas`` 表示传入的透明度数据，可以是单个数也可以是一个数组
+          （对于单个数据，``1`` 表示不透明，``0`` 表示完全透明）
+        - 默认情况下会将所有子物件也设置成指定的颜色，传入 ``root_only=True`` 可以只设置根物件的
+
+        特殊传参：
+
+        - 当 ``colors`` 为四分量 ``RGBA`` 颜色数据时，
+          则同时表示了 ``colors`` 和 ``alphas`` 二者，因此不能再传入 ``alphas`` 参数
+        '''
+        if color is None and alpha is None:
+            return self
+
+        def is_single_color(value: Iterable) -> bool:
+            if isinstance(value, str):
+                return True
+            if isinstance(value[0], str):
+                return False
+            return not isinstance(value[0], Iterable)
+
+        if color is not None and is_single_color(color):
+            color = [color]
+        if alpha is not None and not isinstance(alpha, Iterable):
+            alpha = [alpha]
+
+        if alpha is None and not isinstance(color[0], str) and len(color[0]) == 4:
+            rgbas = self.format_rgbas(color)
+
+            self.set_rgbas(rgbas)
+
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+                cmpt.set_rgbas(rgbas)
+
+        else:
+            if color is not None:
+                color = self.format_colors(color)
+            if alpha is not None:
+                alpha = self.format_alphas(alpha)
+
+            for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+                cmpt_color = cmpt.get()[:, :3] if color is None else color
+                cmpt_alpha = cmpt.get()[:, 3] if alpha is None else alpha
+                length = max(len(cmpt_color), len(cmpt_alpha))
+
+                rgbas = np.hstack([
+                    resize_with_interpolation(cmpt_color.astype(float), length),
+                    resize_with_interpolation(cmpt_alpha.astype(float), length).reshape((length, 1))
+                ])
+                cmpt.set_rgbas(rgbas)
+
+        return self
+
+    def clear(self) -> Self:
+        '''
+        将颜色数据重置为默认值
+        '''
+        self.set(DEFAULT_RGBAS_DATA)
+        return self
+
+    def reverse(self) -> Self:
+        self.set_rgbas(self.get()[::-1])
+        return self
+
+    def resize(self, length: int) -> Self:
+        self.set(resize_with_interpolation(self.get(), max(1, length)))
+        return self
+
+    def count(self) -> int:
+        return len(self.get())
+
+    def apart_alpha(self, n: int) -> Self:
+        '''
+        对每一个颜色数据应用 :func:`~.apart_alpha`
+        '''
+        rgbas = self.get().copy()
+        for i in range(len(rgbas)):
+            rgbas[i, 3] = apart_alpha(rgbas[i, 3], n)
+        self.set_rgbas(rgbas)
+        return self
+
+    def fade(self, factor: float | Iterable[float], *, root_only: bool = False) -> Self:
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            rgbas = cmpt.get().copy()
+            rgbas[:, 3] *= 1 - factor
+            cmpt.set_rgbas(rgbas)
+
+        return self
+
+    # endregion
+
+
+def merge_alpha(alpha: float, n: int) -> float:
+    '''
+    计算透明度 ``alpha`` 在重叠 ``n`` 次混合后的透明度
+    '''
+    result = alpha
+    for _ in range(n - 1):
+        result = 1 - (1 - result) * (1 - alpha)
+
+    return result
+
+
+def apart_alpha(alpha: float, n: int, *, eps: float = 1e-3) -> float:
+    '''
+    将透明度分离为 ``n`` 份，使得这 ``n`` 份混合后仍然表现为原来的透明度
+
+    使得在对齐时产生的重复部分能够更好地渲染
+    '''
+    if alpha >= 1:
+        return 1
+    if alpha <= 0:
+        return 0
+
+    tpl1 = (0, 0)
+    tpl2 = (1, 1)
+
+    # REFACTOR: 有无更好的方式？
+    while tpl2[0] - tpl1[0] > eps:
+        mid_single = (tpl1[0] + tpl2[0]) / 2
+        mid_merged = merge_alpha(mid_single, n)
+        if mid_merged == alpha:
+            return mid_single
+
+        if mid_merged < alpha:
+            tpl1 = (mid_single, mid_merged)
+        else:
+            tpl2 = (mid_single, mid_merged)
+
+    return mid_single
```

### Comparing `janim-1.0.4/janim/components/vpoints.py` & `janim-1.1.0/janim/components/vpoints.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,606 +1,606 @@
-from __future__ import annotations
-
-from enum import Enum
-from typing import Callable, Generator, Iterable, Self
-
-import numpy as np
-
-import janim.utils.refresh as refresh
-from janim.components.points import Cmpt_Points, PointsFn
-from janim.constants import NAN_POINT, ORIGIN, OUT, RIGHT
-from janim.exception import PointError
-from janim.items.item import Item
-from janim.logger import log
-from janim.typing import Vect, VectArray
-from janim.utils.bezier import (PathBuilder,
-                                approx_smooth_quadratic_bezier_handles, bezier,
-                                integer_interpolate, inverse_interpolate,
-                                partial_quadratic_bezier_points,
-                                smooth_quadratic_path)
-from janim.utils.data import AlignedData
-from janim.utils.space_ops import get_norm, get_unit_normal
-
-
-class Cmpt_VPoints[ItemT](Cmpt_Points[ItemT], impl=True):
-    '''
-    曲线点坐标数据
-
-    - 每三个点表示一段二阶贝塞尔曲线，并且前后相接的曲线共用公共点。
-
-      例如对于点坐标列表 ``[a, b, c, d, e, f, g]``，则表示这些曲线：``[a, b, c]`` ``[c, d, e]`` ``[e, f, g]``
-
-    - 将 ``NAN_POINT`` 视为子路径结束的表示。
-
-      例如对于点坐标列表 ``[a, b, c, d, e, NAN_POINT, f, g, h]``，则表示两段子路径：``[a, b, c, d, e]`` 和 ``[f, g, h]``
-
-    - 如果子路径的终止点和起始点相同，则该段子路径被视为闭合路径。
-
-      只有闭合的子路径，才能够进行填充色的渲染
-    '''
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.make_smooth_after_applying_functions = False
-
-    def set(self, points: VectArray) -> Self:
-        if len(points) != 0 and len(points) % 2 == 0:
-            log.warning(f'设置的点数量为 {len(points)}，不是奇数，最后一个点被忽略')
-            points = points[:-1]
-        super().set(points)
-        return self
-
-    def apply_points_fn(
-        self,
-        func: PointsFn,
-        *,
-        about_point: Vect | None = None,
-        about_edge: Vect | None = ORIGIN,
-        root_only: bool = False
-    ) -> Self:
-        super().apply_points_fn(
-            func,
-            about_point=about_point,
-            about_edge=about_edge,
-            root_only=root_only
-        )
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.make_smooth_after_applying_functions:
-                continue
-            cmpt.make_approximately_smooth()
-
-        return self
-
-    # region align
-
-    @classmethod
-    def align_for_interpolate(cls, cmpt1: Cmpt_VPoints, cmpt2: Cmpt_VPoints) -> AlignedData[Self]:
-        cmpt1_copy = cmpt1.copy()
-        cmpt2_copy = cmpt2.copy()
-
-        if cmpt1_copy.not_changed(cmpt2_copy):
-            return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
-
-        if not cmpt1_copy.has():
-            cmpt1_copy.set([cmpt2.self_box.center])
-        if not cmpt2_copy.has():
-            cmpt2_copy.set([cmpt1.self_box.center])
-
-        subpaths1 = cmpt1_copy.get_subpaths()
-        subpaths2 = cmpt2_copy.get_subpaths()
-
-        # 如果都只有单个路径，直接对齐就可以了
-        # 否则进行路径之间的配对，以便对齐数据
-        if len(subpaths1) == len(subpaths2) == 1:
-            sp1, sp2 = cls.align_path(subpaths1[0], subpaths2[0])
-            cmpt1_copy.set(sp1)
-            cmpt2_copy.set(sp2)
-        else:
-            # 这里使得 subpaths1 的子路径数量比 subpaths2 多，简化后面的判断
-            reverse = len(subpaths1) < len(subpaths2)
-            if reverse:
-                cmpt1_copy, cmpt2_copy = cmpt2_copy, cmpt1_copy
-                subpaths1, subpaths2 = subpaths2, subpaths1
-
-            # 用于计算相对距离的“中心”
-            # 这里的 ``RIGHT * (i * 1e-5)`` 是为了是有重合的点有所差别，比如可以保证图形字符 “O” 配对时的一致性
-            def center(i: int, points: np.ndarray) -> np.ndarray:
-                min = np.min(points, axis=0)
-                max = np.max(points, axis=0)
-                return (min + max) * 0.5 + RIGHT * (i * 1e-5)
-
-            # 这里的 ``/ .box.width`` 是为了缩放到一致
-            subpaths1_center = np.array([center(i, subpath) for i, subpath in enumerate(subpaths1)])
-            subpaths1_center -= cmpt1_copy.box.center
-            if cmpt1_copy.box.width != 0:
-                subpaths1_center /= cmpt1_copy.box.width
-            subpaths2_center = np.array([center(i, subpath) for i, subpath in enumerate(subpaths2)])
-            subpaths2_center -= cmpt2_copy.box.center
-            if cmpt2_copy.box.width != 0:
-                subpaths2_center /= cmpt2_copy.box.width
-
-            # 这两个函数使用曼哈顿距离
-            def nearest_idx(point: np.ndarray) -> int:
-                return abs(subpaths2_center - point).sum(axis=1).argmin()
-
-            def sorted_idx(point: np.ndarray) -> Iterable[int]:
-                return abs(subpaths2_center - point).sum(axis=1).argsort()
-
-            type SubPath1Idx = int
-
-            distributions: list[list[SubPath1Idx]] = [[] for _ in range(len(subpaths2))]
-
-            # 将 subpaths1 按照最近原则分配给 subpaths2
-            for idx1, center1 in enumerate(subpaths1_center):
-                distributions[nearest_idx(center1)].append(idx1)
-
-            # 遍历分配结果，如果发现有 subpaths2 中的子路径没有分配到内容，则从其它子路径那边抢一个来
-            for idx2, distri in enumerate(distributions):
-                # 如果有分配到内容，则跳过
-                if distri:
-                    continue
-
-                # 按距离遍历其它的子路径
-                for other_idx in sorted_idx(subpaths2_center[idx2]):
-                    if other_idx == idx2:
-                        continue
-
-                    # 如果其它子路径有两个以上的分配，则从它这里抢一个
-                    other_distri = distributions[other_idx]
-                    if len(other_distri) >= 2:
-                        distri.append(other_distri.pop(0))
-                        break
-
-                # 一定能抢到，所以执行到这里时 distri 应当不为空
-                assert distri
-
-            # 构建新的子路径
-            new_subpaths1 = []
-            new_subpaths2 = []
-
-            for idx2, distri in enumerate(distributions):
-                sp2_orig = subpaths2[idx2]
-
-                # 得到点的数量最匹配的那一组，这样可以尽可能减少插入点的数量
-                diff = np.array([len(subpaths1[idx1]) for idx1 in distri]) - len(sp2_orig)
-                perfect = distri[abs(diff).argmin()]
-
-                for idx1 in distri:
-                    sp1 = subpaths1[idx1]
-                    if idx1 == perfect:
-                        sp2 = sp2_orig
-                    else:
-                        # 对于额外的路径，先创建回环
-                        sp2 = np.vstack([sp2_orig[:-1], sp2_orig[::-1]])
-
-                    sp1, sp2 = cls.align_path(sp1, sp2)
-                    if new_subpaths1:
-                        # 标记前一个路径结束
-                        new_subpaths1.append(NAN_POINT)
-                        new_subpaths2.append(NAN_POINT)
-                    new_subpaths1.append(sp1)
-                    new_subpaths2.append(sp2)
-
-            cmpt1_copy.set(np.vstack(new_subpaths1))
-            cmpt2_copy.set(np.vstack(new_subpaths2))
-
-            # 换回来
-            if reverse:
-                cmpt1_copy, cmpt2_copy = cmpt2_copy, cmpt1_copy
-
-        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
-
-    @staticmethod
-    def align_path(path1: np.ndarray, path2: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
-        diff = abs(len(path1) - len(path2)) // 2
-        if diff == 0:
-            return path1, path2
-
-        return (
-            (Cmpt_VPoints.insert_n_curves_to_point_list(diff, path1), path2)
-            if len(path1) < len(path2)
-            else (path1, Cmpt_VPoints.insert_n_curves_to_point_list(diff, path2))
-        )
-
-    @staticmethod
-    def insert_n_curves_to_point_list(n: int, points: VectArray) -> np.ndarray:
-        if len(points) == 1:
-            return np.repeat(points, 2 * n + 1, 0)
-
-        bezier_tuples = list(Cmpt_VPoints.get_bezier_tuples_from_points(points))
-        norms = [
-            0 if np.isnan(tup[1][0]) else get_norm(tup[2] - tup[0])
-            for tup in bezier_tuples
-        ]
-        # Calculate insertions per curve (ipc)
-        ipc = np.zeros(len(bezier_tuples), dtype=int)
-        for _ in range(n):
-            index = np.argmax(norms)
-            ipc[index] += 1
-            norms[index] *= ipc[index] / (ipc[index] + 1)
-
-        new_points = [points[0]]
-        for tup, n_inserts in zip(bezier_tuples, ipc):
-            # What was once a single quadratic curve defined
-            # by "tup" will now be broken into n_inserts + 1
-            # smaller quadratic curves
-            alphas = np.linspace(0, 1, n_inserts + 2)
-            for a1, a2 in zip(alphas, alphas[1:]):
-                new_points.extend(partial_quadratic_bezier_points(tup, a1, a2)[1:])
-
-        return np.vstack(new_points)
-
-    def insert_n_curves(self, n: int, root_only=False) -> Self:
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            if not isinstance(cmpt, Cmpt_VPoints) or cmpt.curves_count() == 0:
-                continue
-            points = cmpt.insert_n_curves_to_point_list(n, cmpt.get())
-            cmpt.set(points)
-
-        return self
-
-    # endregion
-
-    # region anchors and handles
-
-    def get_anchors(self) -> np.ndarray:
-        '''
-        得到曲线的锚点
-        '''
-        return self.get()[::2]
-
-    def get_handles(self) -> np.ndarray:
-        '''
-        得到曲线的控制点
-        '''
-        return self.get()[1::2]
-
-    @property
-    def start_direction(self) -> np.ndarray:
-        points = self._points.data
-        start = points[0]
-        for pos in points[1:]:
-            if not np.isclose(start, pos).all():
-                return pos - start
-        return RIGHT
-
-    @property
-    def end_direction(self) -> np.ndarray:
-        points = self._points.data
-        end = points[-1]
-        for pos in points[-2::-1]:
-            if not np.isclose(end, pos).all():
-                return end - pos
-        return RIGHT
-
-    def close_path(self) -> Self:
-        self._raise_error_if_no_points()
-        indices = self.get_subpath_end_indices()
-        end = self.get_end()
-        if len(indices) == 1:
-            point = self.get_start()
-        else:
-            point = self._points.data[indices[-2] + 2]
-        self.extend([(end + point) * 0.5, point])
-        return self
-
-    @staticmethod
-    def get_bezier_tuples_from_points(points: VectArray) -> Iterable[np.ndarray]:
-        '''
-        由 ``points`` 得到由每一组贝塞尔曲线控制点组成的列表
-
-        例如，对于有 7 个点的 ``points``，返回值是 ``(points[[0, 1, 2]], points[[2, 3, 4]], points[[4, 5, 6]])``
-        '''
-        n_curves = max(0, len(points) - 1) // 2
-        return (points[2 * i: 2 * i + 3] for i in range(n_curves))
-
-    def get_bezier_tuples(self) -> Iterable[np.ndarray]:
-        '''
-        得到由每一组贝塞尔曲线控制点组成的列表，具体参考 :meth:`get_bezier_tuples_from_points`
-        '''
-        return self.get_bezier_tuples_from_points(self.get())
-
-    def curves_count(self) -> int:
-        '''
-        得到曲线数量
-        '''
-        return max(0, self.count() - 1) // 2
-
-    def get_nth_curve_points(self, n: int) -> VectArray:
-        '''
-        得到第 ``n`` 组的贝塞尔曲线控制点 (从 0 开始计数)
-        '''
-        if n < 0 or n >= self.curves_count():
-            raise PointError(f'n 必须是 0~{self.curves_count() - 1} 的值，{n} 无效')
-        return self._points.data[2 * n: 2 * n + 3]
-
-    def get_nth_curve_function(self, n: int) -> Callable[[float], np.ndarray]:
-        '''
-        返回值是第 ``n`` 组贝塞尔曲线的描点函数，传入 [0, 1] 之间的值，得到对应的在曲线上的点
-        '''
-        return bezier(self.get_nth_curve_points(n))
-
-    def quick_point_from_proportion(self, alpha: float) -> np.ndarray:
-        '''
-        相比 :meth:`point_from_proportion` 而言，更快
-
-        但是这里假设所有的曲线都有相同的长度，所以是不准确的
-        '''
-        num_curves = self.curves_count()
-        n, residue = integer_interpolate(0, num_curves, alpha)
-        curve_func = self.get_nth_curve_function(n)
-        return curve_func(residue)
-
-    def curve_and_prop_of_partial_point(self, alpha: float) -> tuple[int, float]:
-        '''
-        如果你想要得到沿着整个曲线上所在比例为 alpha 处的点，
-        这个函数会返回这个比例所对应的曲线部分的索引，以及在这个曲线部分上需要行进的比例
-        '''
-        if alpha == 0:
-            return (0, 0.0)
-        partials: list[float] = [0]
-        for tup in self.get_bezier_tuples():
-            if (tup[0] == tup[1]).all():
-                # Don't consider null curves
-                arclen = 0
-            else:
-                # Approximate length with straight line from start to end
-                arclen = get_norm(tup[2] - tup[0])
-            partials.append(partials[-1] + arclen)
-        full = partials[-1]
-        if full == 0:
-            return len(partials), 1.0
-        # First index where the partial length is more than alpha times the full length
-        index = next(
-            (i for i, x in enumerate(partials) if x >= full * alpha),
-            len(partials) - 1  # Default
-        )
-        residue = float(inverse_interpolate(
-            partials[index - 1] / full, partials[index] / full, alpha
-        ))
-        return index - 1, residue
-
-    def point_from_proportion(self, alpha: float) -> np.ndarray:
-        if alpha <= 0:
-            return self.get_start()
-        elif alpha >= 1:
-            return self.get_end()
-        index, residue = self.curve_and_prop_of_partial_point(alpha)
-        return self.get_nth_curve_function(index)(residue)
-
-    def pointwise_become_partial(self, other: Cmpt_VPoints | Item, a: float, b: float) -> Self:
-        if isinstance(other, Item):
-            cmpt = self.get_same_cmpt(other)
-        else:
-            cmpt = other
-
-        points = cmpt.get()
-        if a <= 0 and b >= 1:
-            self.set(points)
-            return self
-        num_curves = cmpt.curves_count()
-
-        # Partial curve includes three portions:
-        # - A start, which is some ending portion of an inner quadratic
-        # - A middle section, which matches the curve exactly
-        # - An end, which is the starting portion of a later inner quadratic
-
-        lower_index, lower_residue = integer_interpolate(0, num_curves, a)
-        upper_index, upper_residue = integer_interpolate(0, num_curves, b)
-        i1 = 2 * lower_index
-        i2 = 2 * lower_index + 3
-        i3 = 2 * upper_index
-        i4 = 2 * upper_index + 3
-
-        new_points = points.copy()
-        if num_curves == 0:
-            new_points[:] = 0
-            return self
-        if lower_index == upper_index:
-            tup = partial_quadratic_bezier_points(points[i1:i2], lower_residue, upper_residue)
-            new_points[:i1] = tup[0]
-            new_points[i1:i4] = tup
-            new_points[i4:] = tup[2]
-        else:
-            low_tup = partial_quadratic_bezier_points(points[i1:i2], lower_residue, 1)
-            high_tup = partial_quadratic_bezier_points(points[i3:i4], 0, upper_residue)
-            new_points[0:i1] = low_tup[0]
-            new_points[i1:i2] = low_tup
-            # Keep new_points i2:i3 as they are
-            new_points[i3:i4] = high_tup
-            new_points[i4:] = high_tup[2]
-        self.set(new_points)
-        return self
-
-    # endregion
-
-    # region _as_corners 操作
-
-    def add_as_corners(self, points: VectArray) -> Self:
-        '''
-        以折线的方式将 ``points`` 添加
-        '''
-        if not self.has():
-            self.set(points[0])
-
-        builder = PathBuilder(start_point=self.get_end())
-        for point in points:
-            builder.line_to(point)
-        self.extend(builder.get()[1:])
-
-        return self
-
-    def set_as_corners(self, points: VectArray) -> Self:
-        '''
-        将点数据设置为由 ``points`` 构成的折线
-        '''
-        builder = PathBuilder(start_point=points[0])
-        for point in points[1:]:
-            builder.line_to(point)
-        self.set(builder.get())
-
-    # endregion
-
-    # region anchor mode
-
-    # TODO: is_smooth
-
-    def change_anchor_mode(self, mode: AnchorMode) -> Self:
-        if not self.has():
-            return self
-
-        subpaths = self.get_subpaths()
-        self.clear()
-        for subpath in subpaths:
-            new_subpath = subpath.copy()
-            anchors = subpath[::2]
-            match mode:
-                case AnchorMode.Jagged:
-                    new_subpath[1::2] = 0.5 * (anchors[:-1] + anchors[1:])
-                case AnchorMode.ApproxSmooth:
-                    new_subpath[1::2] = approx_smooth_quadratic_bezier_handles(anchors)
-                case AnchorMode.TrueSmooth:
-                    new_subpath = smooth_quadratic_path(anchors)
-            self.add_subpath(new_subpath)
-        return self
-
-    def make_smooth(self, approx=False, root_only=False) -> Self:
-        '''
-        Edits the path so as to pass smoothly through all
-        the current anchor points.
-
-        If approx is False, this may increase the total
-        number of points.
-        '''
-        mode = AnchorMode.ApproxSmooth if approx else AnchorMode.TrueSmooth
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            if not isinstance(cmpt, Cmpt_VPoints):
-                continue
-            cmpt.change_anchor_mode(mode)
-
-        return self
-
-    def make_approximately_smooth(self, root_only=False) -> Self:
-        self.make_smooth(approx=True, root_only=root_only)
-        return self
-
-    def make_jagged(self, root_only=False) -> Self:
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            if not isinstance(cmpt, Cmpt_VPoints):
-                continue
-            cmpt.change_anchor_mode(AnchorMode.Jagged)
-
-        return self
-
-    # endregion
-
-    # region unit_normal
-
-    @staticmethod
-    def get_area_vector_from_points(points: np.ndarray) -> np.ndarray:
-        if len(points) == 0:
-            return np.zeros(3)
-
-        p0 = points[::2]
-        p1 = np.roll(p0, -1, axis=0)
-
-        # Each term goes through all edges [(x0, y0, z0), (x1, y1, z1)]
-        sums = p0 + p1
-        diffs = p1 - p0
-        return 0.5 * np.array([
-            (sums[:, 1] * diffs[:, 2]).sum(),  # Add up (y0 + y1)*(z1 - z0)
-            (sums[:, 2] * diffs[:, 0]).sum(),  # Add up (z0 + z1)*(x1 - x0)
-            (sums[:, 0] * diffs[:, 1]).sum(),  # Add up (x0 + x1)*(y1 - y0)
-        ])
-
-    @property
-    @Cmpt_Points.set.self_refresh()
-    @refresh.register
-    def area_vector(self) -> np.ndarray:
-        '''
-        一个向量，其长度为锚点形成的多边形所围成的面积，根据右手定则指向垂直于该多边形的方向
-        '''
-        return self.get_area_vector_from_points(self.get())
-
-    @property
-    @Cmpt_Points.set.self_refresh()
-    @refresh.register
-    def unit_normal(self) -> np.ndarray:
-        if self.count() < 3:
-            return OUT
-
-        area_vect = self.area_vector
-        area = get_norm(area_vect)
-        if area > 0:
-            return area_vect / area
-
-        points = self.get()
-        return get_unit_normal(
-            points[1] - points[0],
-            points[2] - points[1]
-        )
-
-    # endregion
-
-    # region subpaths
-
-    def walk_subpath_end_indices(self) -> Generator[int, None, None]:
-        '''
-        遍历每个子路径结尾的下标
-        '''
-        points = self.get()
-        handles = points[1::2]
-        yield from np.where(np.isnan(handles[:, 0]))[0] * 2
-        yield len(points) - 1
-
-    def get_subpath_end_indices(self) -> list[int]:
-        return list(self.walk_subpath_end_indices())
-
-    def get_closepath_flags(self) -> np.ndarray:
-        '''
-        得到子路径是否闭合的标志，结果长度与点数量相同
-
-        对于闭合路径，结果中对应部分会被设置为 ``True``
-        '''
-        result = np.full(self.count(), False)
-        if len(result) == 0:
-            return result
-
-        points = self.get()
-
-        start_idx = 0
-        for end_idx in self.walk_subpath_end_indices():
-            if np.isclose(points[end_idx], points[start_idx]).all():
-                result[start_idx: end_idx + 1] = True
-            start_idx = end_idx + 2
-
-        return result
-
-    @staticmethod
-    def get_parts_by_end_indices(array: np.ndarray, end_indices: np.ndarray) -> list[np.ndarray]:
-        '''
-        根据子路径结尾下标的列表，将 ``array`` 分段
-        '''
-        if len(array) == 0:
-            return []
-        start_indices = [0, *(end_indices[:-1] + 2)]
-        return [array[i1: i2 + 1] for i1, i2 in zip(start_indices, end_indices)]
-
-    def get_subpaths(self) -> list[np.ndarray]:
-        '''
-        得到子路径列表
-        '''
-        return self.get_parts_by_end_indices(self.get(), np.array(self.get_subpath_end_indices()))
-
-    def add_subpath(self, points: VectArray) -> Self:
-        if not self.has():
-            self.set(points)
-        else:
-            self.extend([NAN_POINT, *points])
-        return self
-
-    # endregion
-
-
-class AnchorMode(Enum):
-    Jagged = 0
-    ApproxSmooth = 1
-    TrueSmooth = 2
+from __future__ import annotations
+
+from enum import Enum
+from typing import Callable, Generator, Iterable, Self
+
+import numpy as np
+
+import janim.utils.refresh as refresh
+from janim.components.points import Cmpt_Points, PointsFn
+from janim.constants import NAN_POINT, ORIGIN, OUT, RIGHT
+from janim.exception import PointError
+from janim.items.item import Item
+from janim.logger import log
+from janim.typing import Vect, VectArray
+from janim.utils.bezier import (PathBuilder,
+                                approx_smooth_quadratic_bezier_handles, bezier,
+                                integer_interpolate, inverse_interpolate,
+                                partial_quadratic_bezier_points,
+                                smooth_quadratic_path)
+from janim.utils.data import AlignedData
+from janim.utils.space_ops import get_norm, get_unit_normal
+
+
+class Cmpt_VPoints[ItemT](Cmpt_Points[ItemT], impl=True):
+    '''
+    曲线点坐标数据
+
+    - 每三个点表示一段二阶贝塞尔曲线，并且前后相接的曲线共用公共点。
+
+      例如对于点坐标列表 ``[a, b, c, d, e, f, g]``，则表示这些曲线：``[a, b, c]`` ``[c, d, e]`` ``[e, f, g]``
+
+    - 将 ``NAN_POINT`` 视为子路径结束的表示。
+
+      例如对于点坐标列表 ``[a, b, c, d, e, NAN_POINT, f, g, h]``，则表示两段子路径：``[a, b, c, d, e]`` 和 ``[f, g, h]``
+
+    - 如果子路径的终止点和起始点相同，则该段子路径被视为闭合路径。
+
+      只有闭合的子路径，才能够进行填充色的渲染
+    '''
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.make_smooth_after_applying_functions = False
+
+    def set(self, points: VectArray) -> Self:
+        if len(points) != 0 and len(points) % 2 == 0:
+            log.warning(f'设置的点数量为 {len(points)}，不是奇数，最后一个点被忽略')
+            points = points[:-1]
+        super().set(points)
+        return self
+
+    def apply_points_fn(
+        self,
+        func: PointsFn,
+        *,
+        about_point: Vect | None = None,
+        about_edge: Vect | None = ORIGIN,
+        root_only: bool = False
+    ) -> Self:
+        super().apply_points_fn(
+            func,
+            about_point=about_point,
+            about_edge=about_edge,
+            root_only=root_only
+        )
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.make_smooth_after_applying_functions:
+                continue
+            cmpt.make_approximately_smooth()
+
+        return self
+
+    # region align
+
+    @classmethod
+    def align_for_interpolate(cls, cmpt1: Cmpt_VPoints, cmpt2: Cmpt_VPoints) -> AlignedData[Self]:
+        cmpt1_copy = cmpt1.copy()
+        cmpt2_copy = cmpt2.copy()
+
+        if cmpt1_copy.not_changed(cmpt2_copy):
+            return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
+
+        if not cmpt1_copy.has():
+            cmpt1_copy.set([cmpt2.self_box.center])
+        if not cmpt2_copy.has():
+            cmpt2_copy.set([cmpt1.self_box.center])
+
+        subpaths1 = cmpt1_copy.get_subpaths()
+        subpaths2 = cmpt2_copy.get_subpaths()
+
+        # 如果都只有单个路径，直接对齐就可以了
+        # 否则进行路径之间的配对，以便对齐数据
+        if len(subpaths1) == len(subpaths2) == 1:
+            sp1, sp2 = cls.align_path(subpaths1[0], subpaths2[0])
+            cmpt1_copy.set(sp1)
+            cmpt2_copy.set(sp2)
+        else:
+            # 这里使得 subpaths1 的子路径数量比 subpaths2 多，简化后面的判断
+            reverse = len(subpaths1) < len(subpaths2)
+            if reverse:
+                cmpt1_copy, cmpt2_copy = cmpt2_copy, cmpt1_copy
+                subpaths1, subpaths2 = subpaths2, subpaths1
+
+            # 用于计算相对距离的“中心”
+            # 这里的 ``RIGHT * (i * 1e-5)`` 是为了是有重合的点有所差别，比如可以保证图形字符 “O” 配对时的一致性
+            def center(i: int, points: np.ndarray) -> np.ndarray:
+                min = np.min(points, axis=0)
+                max = np.max(points, axis=0)
+                return (min + max) * 0.5 + RIGHT * (i * 1e-5)
+
+            # 这里的 ``/ .box.width`` 是为了缩放到一致
+            subpaths1_center = np.array([center(i, subpath) for i, subpath in enumerate(subpaths1)])
+            subpaths1_center -= cmpt1_copy.box.center
+            if cmpt1_copy.box.width != 0:
+                subpaths1_center /= cmpt1_copy.box.width
+            subpaths2_center = np.array([center(i, subpath) for i, subpath in enumerate(subpaths2)])
+            subpaths2_center -= cmpt2_copy.box.center
+            if cmpt2_copy.box.width != 0:
+                subpaths2_center /= cmpt2_copy.box.width
+
+            # 这两个函数使用曼哈顿距离
+            def nearest_idx(point: np.ndarray) -> int:
+                return abs(subpaths2_center - point).sum(axis=1).argmin()
+
+            def sorted_idx(point: np.ndarray) -> Iterable[int]:
+                return abs(subpaths2_center - point).sum(axis=1).argsort()
+
+            type SubPath1Idx = int
+
+            distributions: list[list[SubPath1Idx]] = [[] for _ in range(len(subpaths2))]
+
+            # 将 subpaths1 按照最近原则分配给 subpaths2
+            for idx1, center1 in enumerate(subpaths1_center):
+                distributions[nearest_idx(center1)].append(idx1)
+
+            # 遍历分配结果，如果发现有 subpaths2 中的子路径没有分配到内容，则从其它子路径那边抢一个来
+            for idx2, distri in enumerate(distributions):
+                # 如果有分配到内容，则跳过
+                if distri:
+                    continue
+
+                # 按距离遍历其它的子路径
+                for other_idx in sorted_idx(subpaths2_center[idx2]):
+                    if other_idx == idx2:
+                        continue
+
+                    # 如果其它子路径有两个以上的分配，则从它这里抢一个
+                    other_distri = distributions[other_idx]
+                    if len(other_distri) >= 2:
+                        distri.append(other_distri.pop(0))
+                        break
+
+                # 一定能抢到，所以执行到这里时 distri 应当不为空
+                assert distri
+
+            # 构建新的子路径
+            new_subpaths1 = []
+            new_subpaths2 = []
+
+            for idx2, distri in enumerate(distributions):
+                sp2_orig = subpaths2[idx2]
+
+                # 得到点的数量最匹配的那一组，这样可以尽可能减少插入点的数量
+                diff = np.array([len(subpaths1[idx1]) for idx1 in distri]) - len(sp2_orig)
+                perfect = distri[abs(diff).argmin()]
+
+                for idx1 in distri:
+                    sp1 = subpaths1[idx1]
+                    if idx1 == perfect:
+                        sp2 = sp2_orig
+                    else:
+                        # 对于额外的路径，先创建回环
+                        sp2 = np.vstack([sp2_orig[:-1], sp2_orig[::-1]])
+
+                    sp1, sp2 = cls.align_path(sp1, sp2)
+                    if new_subpaths1:
+                        # 标记前一个路径结束
+                        new_subpaths1.append(NAN_POINT)
+                        new_subpaths2.append(NAN_POINT)
+                    new_subpaths1.append(sp1)
+                    new_subpaths2.append(sp2)
+
+            cmpt1_copy.set(np.vstack(new_subpaths1))
+            cmpt2_copy.set(np.vstack(new_subpaths2))
+
+            # 换回来
+            if reverse:
+                cmpt1_copy, cmpt2_copy = cmpt2_copy, cmpt1_copy
+
+        return AlignedData(cmpt1_copy, cmpt2_copy, cmpt1_copy.copy())
+
+    @staticmethod
+    def align_path(path1: np.ndarray, path2: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+        diff = abs(len(path1) - len(path2)) // 2
+        if diff == 0:
+            return path1, path2
+
+        return (
+            (Cmpt_VPoints.insert_n_curves_to_point_list(diff, path1), path2)
+            if len(path1) < len(path2)
+            else (path1, Cmpt_VPoints.insert_n_curves_to_point_list(diff, path2))
+        )
+
+    @staticmethod
+    def insert_n_curves_to_point_list(n: int, points: VectArray) -> np.ndarray:
+        if len(points) == 1:
+            return np.repeat(points, 2 * n + 1, 0)
+
+        bezier_tuples = list(Cmpt_VPoints.get_bezier_tuples_from_points(points))
+        norms = [
+            0 if np.isnan(tup[1][0]) else get_norm(tup[2] - tup[0])
+            for tup in bezier_tuples
+        ]
+        # Calculate insertions per curve (ipc)
+        ipc = np.zeros(len(bezier_tuples), dtype=int)
+        for _ in range(n):
+            index = np.argmax(norms)
+            ipc[index] += 1
+            norms[index] *= ipc[index] / (ipc[index] + 1)
+
+        new_points = [points[0]]
+        for tup, n_inserts in zip(bezier_tuples, ipc):
+            # What was once a single quadratic curve defined
+            # by "tup" will now be broken into n_inserts + 1
+            # smaller quadratic curves
+            alphas = np.linspace(0, 1, n_inserts + 2)
+            for a1, a2 in zip(alphas, alphas[1:]):
+                new_points.extend(partial_quadratic_bezier_points(tup, a1, a2)[1:])
+
+        return np.vstack(new_points)
+
+    def insert_n_curves(self, n: int, root_only=False) -> Self:
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or cmpt.curves_count() == 0:
+                continue
+            points = cmpt.insert_n_curves_to_point_list(n, cmpt.get())
+            cmpt.set(points)
+
+        return self
+
+    # endregion
+
+    # region anchors and handles
+
+    def get_anchors(self) -> np.ndarray:
+        '''
+        得到曲线的锚点
+        '''
+        return self.get()[::2]
+
+    def get_handles(self) -> np.ndarray:
+        '''
+        得到曲线的控制点
+        '''
+        return self.get()[1::2]
+
+    @property
+    def start_direction(self) -> np.ndarray:
+        points = self._points.data
+        start = points[0]
+        for pos in points[1:]:
+            if not np.isclose(start, pos).all():
+                return pos - start
+        return RIGHT
+
+    @property
+    def end_direction(self) -> np.ndarray:
+        points = self._points.data
+        end = points[-1]
+        for pos in points[-2::-1]:
+            if not np.isclose(end, pos).all():
+                return end - pos
+        return RIGHT
+
+    def close_path(self) -> Self:
+        self._raise_error_if_no_points()
+        indices = self.get_subpath_end_indices()
+        end = self.get_end()
+        if len(indices) == 1:
+            point = self.get_start()
+        else:
+            point = self._points.data[indices[-2] + 2]
+        self.extend([(end + point) * 0.5, point])
+        return self
+
+    @staticmethod
+    def get_bezier_tuples_from_points(points: VectArray) -> Iterable[np.ndarray]:
+        '''
+        由 ``points`` 得到由每一组贝塞尔曲线控制点组成的列表
+
+        例如，对于有 7 个点的 ``points``，返回值是 ``(points[[0, 1, 2]], points[[2, 3, 4]], points[[4, 5, 6]])``
+        '''
+        n_curves = max(0, len(points) - 1) // 2
+        return (points[2 * i: 2 * i + 3] for i in range(n_curves))
+
+    def get_bezier_tuples(self) -> Iterable[np.ndarray]:
+        '''
+        得到由每一组贝塞尔曲线控制点组成的列表，具体参考 :meth:`get_bezier_tuples_from_points`
+        '''
+        return self.get_bezier_tuples_from_points(self.get())
+
+    def curves_count(self) -> int:
+        '''
+        得到曲线数量
+        '''
+        return max(0, self.count() - 1) // 2
+
+    def get_nth_curve_points(self, n: int) -> VectArray:
+        '''
+        得到第 ``n`` 组的贝塞尔曲线控制点 (从 0 开始计数)
+        '''
+        if n < 0 or n >= self.curves_count():
+            raise PointError(f'n 必须是 0~{self.curves_count() - 1} 的值，{n} 无效')
+        return self._points.data[2 * n: 2 * n + 3]
+
+    def get_nth_curve_function(self, n: int) -> Callable[[float], np.ndarray]:
+        '''
+        返回值是第 ``n`` 组贝塞尔曲线的描点函数，传入 [0, 1] 之间的值，得到对应的在曲线上的点
+        '''
+        return bezier(self.get_nth_curve_points(n))
+
+    def quick_point_from_proportion(self, alpha: float) -> np.ndarray:
+        '''
+        相比 :meth:`point_from_proportion` 而言，更快
+
+        但是这里假设所有的曲线都有相同的长度，所以是不准确的
+        '''
+        num_curves = self.curves_count()
+        n, residue = integer_interpolate(0, num_curves, alpha)
+        curve_func = self.get_nth_curve_function(n)
+        return curve_func(residue)
+
+    def curve_and_prop_of_partial_point(self, alpha: float) -> tuple[int, float]:
+        '''
+        如果你想要得到沿着整个曲线上所在比例为 alpha 处的点，
+        这个函数会返回这个比例所对应的曲线部分的索引，以及在这个曲线部分上需要行进的比例
+        '''
+        if alpha == 0:
+            return (0, 0.0)
+        partials: list[float] = [0]
+        for tup in self.get_bezier_tuples():
+            if (tup[0] == tup[1]).all():
+                # Don't consider null curves
+                arclen = 0
+            else:
+                # Approximate length with straight line from start to end
+                arclen = get_norm(tup[2] - tup[0])
+            partials.append(partials[-1] + arclen)
+        full = partials[-1]
+        if full == 0:
+            return len(partials), 1.0
+        # First index where the partial length is more than alpha times the full length
+        index = next(
+            (i for i, x in enumerate(partials) if x >= full * alpha),
+            len(partials) - 1  # Default
+        )
+        residue = float(inverse_interpolate(
+            partials[index - 1] / full, partials[index] / full, alpha
+        ))
+        return index - 1, residue
+
+    def point_from_proportion(self, alpha: float) -> np.ndarray:
+        if alpha <= 0:
+            return self.get_start()
+        elif alpha >= 1:
+            return self.get_end()
+        index, residue = self.curve_and_prop_of_partial_point(alpha)
+        return self.get_nth_curve_function(index)(residue)
+
+    def pointwise_become_partial(self, other: Cmpt_VPoints | Item, a: float, b: float) -> Self:
+        if isinstance(other, Item):
+            cmpt = self.get_same_cmpt(other)
+        else:
+            cmpt = other
+
+        points = cmpt.get()
+        if a <= 0 and b >= 1:
+            self.set(points)
+            return self
+        num_curves = cmpt.curves_count()
+
+        # Partial curve includes three portions:
+        # - A start, which is some ending portion of an inner quadratic
+        # - A middle section, which matches the curve exactly
+        # - An end, which is the starting portion of a later inner quadratic
+
+        lower_index, lower_residue = integer_interpolate(0, num_curves, a)
+        upper_index, upper_residue = integer_interpolate(0, num_curves, b)
+        i1 = 2 * lower_index
+        i2 = 2 * lower_index + 3
+        i3 = 2 * upper_index
+        i4 = 2 * upper_index + 3
+
+        new_points = points.copy()
+        if num_curves == 0:
+            new_points[:] = 0
+            return self
+        if lower_index == upper_index:
+            tup = partial_quadratic_bezier_points(points[i1:i2], lower_residue, upper_residue)
+            new_points[:i1] = tup[0]
+            new_points[i1:i4] = tup
+            new_points[i4:] = tup[2]
+        else:
+            low_tup = partial_quadratic_bezier_points(points[i1:i2], lower_residue, 1)
+            high_tup = partial_quadratic_bezier_points(points[i3:i4], 0, upper_residue)
+            new_points[0:i1] = low_tup[0]
+            new_points[i1:i2] = low_tup
+            # Keep new_points i2:i3 as they are
+            new_points[i3:i4] = high_tup
+            new_points[i4:] = high_tup[2]
+        self.set(new_points)
+        return self
+
+    # endregion
+
+    # region _as_corners 操作
+
+    def add_as_corners(self, points: VectArray) -> Self:
+        '''
+        以折线的方式将 ``points`` 添加
+        '''
+        if not self.has():
+            self.set(points[0])
+
+        builder = PathBuilder(start_point=self.get_end())
+        for point in points:
+            builder.line_to(point)
+        self.extend(builder.get()[1:])
+
+        return self
+
+    def set_as_corners(self, points: VectArray) -> Self:
+        '''
+        将点数据设置为由 ``points`` 构成的折线
+        '''
+        builder = PathBuilder(start_point=points[0])
+        for point in points[1:]:
+            builder.line_to(point)
+        self.set(builder.get())
+
+    # endregion
+
+    # region anchor mode
+
+    # TODO: is_smooth
+
+    def change_anchor_mode(self, mode: AnchorMode) -> Self:
+        if not self.has():
+            return self
+
+        subpaths = self.get_subpaths()
+        self.clear()
+        for subpath in subpaths:
+            new_subpath = subpath.copy()
+            anchors = subpath[::2]
+            match mode:
+                case AnchorMode.Jagged:
+                    new_subpath[1::2] = 0.5 * (anchors[:-1] + anchors[1:])
+                case AnchorMode.ApproxSmooth:
+                    new_subpath[1::2] = approx_smooth_quadratic_bezier_handles(anchors)
+                case AnchorMode.TrueSmooth:
+                    new_subpath = smooth_quadratic_path(anchors)
+            self.add_subpath(new_subpath)
+        return self
+
+    def make_smooth(self, approx=False, root_only=False) -> Self:
+        '''
+        Edits the path so as to pass smoothly through all
+        the current anchor points.
+
+        If approx is False, this may increase the total
+        number of points.
+        '''
+        mode = AnchorMode.ApproxSmooth if approx else AnchorMode.TrueSmooth
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints):
+                continue
+            cmpt.change_anchor_mode(mode)
+
+        return self
+
+    def make_approximately_smooth(self, root_only=False) -> Self:
+        self.make_smooth(approx=True, root_only=root_only)
+        return self
+
+    def make_jagged(self, root_only=False) -> Self:
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints):
+                continue
+            cmpt.change_anchor_mode(AnchorMode.Jagged)
+
+        return self
+
+    # endregion
+
+    # region unit_normal
+
+    @staticmethod
+    def get_area_vector_from_points(points: np.ndarray) -> np.ndarray:
+        if len(points) == 0:
+            return np.zeros(3)
+
+        p0 = points[::2]
+        p1 = np.roll(p0, -1, axis=0)
+
+        # Each term goes through all edges [(x0, y0, z0), (x1, y1, z1)]
+        sums = p0 + p1
+        diffs = p1 - p0
+        return 0.5 * np.array([
+            (sums[:, 1] * diffs[:, 2]).sum(),  # Add up (y0 + y1)*(z1 - z0)
+            (sums[:, 2] * diffs[:, 0]).sum(),  # Add up (z0 + z1)*(x1 - x0)
+            (sums[:, 0] * diffs[:, 1]).sum(),  # Add up (x0 + x1)*(y1 - y0)
+        ])
+
+    @property
+    @Cmpt_Points.set.self_refresh()
+    @refresh.register
+    def area_vector(self) -> np.ndarray:
+        '''
+        一个向量，其长度为锚点形成的多边形所围成的面积，根据右手定则指向垂直于该多边形的方向
+        '''
+        return self.get_area_vector_from_points(self.get())
+
+    @property
+    @Cmpt_Points.set.self_refresh()
+    @refresh.register
+    def unit_normal(self) -> np.ndarray:
+        if self.count() < 3:
+            return OUT
+
+        area_vect = self.area_vector
+        area = get_norm(area_vect)
+        if area > 0:
+            return area_vect / area
+
+        points = self.get()
+        return get_unit_normal(
+            points[1] - points[0],
+            points[2] - points[1]
+        )
+
+    # endregion
+
+    # region subpaths
+
+    def walk_subpath_end_indices(self) -> Generator[int, None, None]:
+        '''
+        遍历每个子路径结尾的下标
+        '''
+        points = self.get()
+        handles = points[1::2]
+        yield from np.where(np.isnan(handles[:, 0]))[0] * 2
+        yield len(points) - 1
+
+    def get_subpath_end_indices(self) -> list[int]:
+        return list(self.walk_subpath_end_indices())
+
+    def get_closepath_flags(self) -> np.ndarray:
+        '''
+        得到子路径是否闭合的标志，结果长度与点数量相同
+
+        对于闭合路径，结果中对应部分会被设置为 ``True``
+        '''
+        result = np.full(self.count(), False)
+        if len(result) == 0:
+            return result
+
+        points = self.get()
+
+        start_idx = 0
+        for end_idx in self.walk_subpath_end_indices():
+            if np.isclose(points[end_idx], points[start_idx]).all():
+                result[start_idx: end_idx + 1] = True
+            start_idx = end_idx + 2
+
+        return result
+
+    @staticmethod
+    def get_parts_by_end_indices(array: np.ndarray, end_indices: np.ndarray) -> list[np.ndarray]:
+        '''
+        根据子路径结尾下标的列表，将 ``array`` 分段
+        '''
+        if len(array) == 0:
+            return []
+        start_indices = [0, *(end_indices[:-1] + 2)]
+        return [array[i1: i2 + 1] for i1, i2 in zip(start_indices, end_indices)]
+
+    def get_subpaths(self) -> list[np.ndarray]:
+        '''
+        得到子路径列表
+        '''
+        return self.get_parts_by_end_indices(self.get(), np.array(self.get_subpath_end_indices()))
+
+    def add_subpath(self, points: VectArray) -> Self:
+        if not self.has():
+            self.set(points)
+        else:
+            self.extend([NAN_POINT, *points])
+        return self
+
+    # endregion
+
+
+class AnchorMode(Enum):
+    Jagged = 0
+    ApproxSmooth = 1
+    TrueSmooth = 2
```

### Comparing `janim-1.0.4/janim/constants/coord.py` & `janim-1.1.0/janim/constants/coord.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import numpy as np
-
-ORIGIN = np.array((0., 0., 0.))
-UP = np.array((0., 1., 0.))
-DOWN = np.array((0., -1., 0.))
-RIGHT = np.array((1., 0., 0.))
-LEFT = np.array((-1., 0., 0.))
-IN = np.array((0., 0., -1.))
-OUT = np.array((0., 0., 1.))
-X_AXIS = np.array((1., 0., 0.))
-Y_AXIS = np.array((0., 1., 0.))
-Z_AXIS = np.array((0., 0., 1.))
-
-NAN_POINT = np.full(3, np.nan)
-
-# Useful abbreviations for diagonals
-UL = UP + LEFT
-UR = UP + RIGHT
-DL = DOWN + LEFT
-DR = DOWN + RIGHT
-
-for p in (ORIGIN, UP, DOWN, RIGHT, LEFT, IN, OUT,
-          X_AXIS, Y_AXIS, Z_AXIS, NAN_POINT,
-          UL, UR, DL, DR):
-    p.setflags(write=False)
+import numpy as np
+
+ORIGIN = np.array((0., 0., 0.))
+UP = np.array((0., 1., 0.))
+DOWN = np.array((0., -1., 0.))
+RIGHT = np.array((1., 0., 0.))
+LEFT = np.array((-1., 0., 0.))
+IN = np.array((0., 0., -1.))
+OUT = np.array((0., 0., 1.))
+X_AXIS = np.array((1., 0., 0.))
+Y_AXIS = np.array((0., 1., 0.))
+Z_AXIS = np.array((0., 0., 1.))
+
+NAN_POINT = np.full(3, np.nan)
+
+# Useful abbreviations for diagonals
+UL = UP + LEFT
+UR = UP + RIGHT
+DL = DOWN + LEFT
+DR = DOWN + RIGHT
+
+for p in (ORIGIN, UP, DOWN, RIGHT, LEFT, IN, OUT,
+          X_AXIS, Y_AXIS, Z_AXIS, NAN_POINT,
+          UL, UR, DL, DR):
+    p.setflags(write=False)
```

### Comparing `janim-1.0.4/janim/exception.py` & `janim-1.1.0/janim/exception.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import sys
-from dataclasses import dataclass
-
-
-_sys_excepthook = sys.excepthook
-
-
-def custom_excepthook(exc_type, exc_value, exc_traceback):
-    if issubclass(exc_type, ExitException):
-        sys.exit(exc_value.exit_code)
-    _sys_excepthook(exc_type, exc_value, exc_traceback)
-
-
-sys.excepthook = custom_excepthook
-
-
-EXITCODE_PYSIDE6_NOT_FOUND = 1001
-'''``PySide6`` 未安装时的退出码'''
-EXITCODE_MODULE_NOT_FOUND = 1002
-'''使用 ``run`` 或 ``write`` 指定的文件未找到时的退出码'''
-EXITCODE_NOT_FILE = 1003
-'''使用 ``run`` 或 ``write`` 指定路径不是文件时的退出码'''
-
-EXITCODE_TYPST_NOT_FOUND = 1101
-'''``Typst`` 未安装时的退出码'''
-EXITCODE_TYPST_COMPILE_ERROR = 1102
-'''``Typst`` 编译失败时的退出码'''
-
-EXITCODE_FFMPEG_NOT_FOUND = 2001
-'''``ffmpeg`` 未安装时的退出码'''
-
-
-class JAnimException(Exception): ...
-
-
-@dataclass
-class ExitException(JAnimException):
-    '''
-    当 :class:`ExitException` 未被捕获时，
-    会直接以 ``exit_code`` 退出，不输出 ``traceback`` 信息
-    '''
-    exit_code: int
-
-
-class TimelineError(JAnimException): ...
-class TimelineLookupError(TimelineError): ...
-class RecordFailedError(TimelineError): ...
-class RecordNotFoundError(TimelineError): ...
-class NotAnimationError(TimelineError): ...
-
-
-class UpdaterError(JAnimException): ...
-
-
-class CmptGroupLookupError(JAnimException): ...
-
-
-class PointError(JAnimException): ...
-class InvaildMatrixError(PointError): ...
-
-
-class BooleanOpsError(JAnimException): ...
-
-
-class AsTypeError(JAnimException): ...
-
-
-class ColorNotFoundError(JAnimException): ...
-class FontNotFoundError(JAnimException): ...
+import sys
+from dataclasses import dataclass
+
+
+_sys_excepthook = sys.excepthook
+
+
+def custom_excepthook(exc_type, exc_value, exc_traceback):
+    if issubclass(exc_type, ExitException):
+        sys.exit(exc_value.exit_code)
+    _sys_excepthook(exc_type, exc_value, exc_traceback)
+
+
+sys.excepthook = custom_excepthook
+
+
+EXITCODE_PYSIDE6_NOT_FOUND = 1001
+'''``PySide6`` 未安装时的退出码'''
+EXITCODE_MODULE_NOT_FOUND = 1002
+'''使用 ``run`` 或 ``write`` 指定的文件未找到时的退出码'''
+EXITCODE_NOT_FILE = 1003
+'''使用 ``run`` 或 ``write`` 指定路径不是文件时的退出码'''
+
+EXITCODE_TYPST_NOT_FOUND = 1101
+'''``Typst`` 未安装时的退出码'''
+EXITCODE_TYPST_COMPILE_ERROR = 1102
+'''``Typst`` 编译失败时的退出码'''
+
+EXITCODE_FFMPEG_NOT_FOUND = 2001
+'''``ffmpeg`` 未安装时的退出码'''
+
+
+class JAnimException(Exception): ...
+
+
+@dataclass
+class ExitException(JAnimException):
+    '''
+    当 :class:`ExitException` 未被捕获时，
+    会直接以 ``exit_code`` 退出，不输出 ``traceback`` 信息
+    '''
+    exit_code: int
+
+
+class TimelineError(JAnimException): ...
+class TimelineLookupError(TimelineError): ...
+class RecordFailedError(TimelineError): ...
+class RecordNotFoundError(TimelineError): ...
+class NotAnimationError(TimelineError): ...
+
+
+class UpdaterError(JAnimException): ...
+
+
+class CmptGroupLookupError(JAnimException): ...
+
+
+class PointError(JAnimException): ...
+class InvaildMatrixError(PointError): ...
+
+
+class BooleanOpsError(JAnimException): ...
+
+
+class AsTypeError(JAnimException): ...
+
+
+class ColorNotFoundError(JAnimException): ...
+class FontNotFoundError(JAnimException): ...
```

### Comparing `janim-1.0.4/janim/gui/export.png` & `janim-1.1.0/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.4/janim/gui/favicon.ico` & `janim-1.1.0/janim/gui/favicon.ico`

 * *Files identical despite different names*

### Comparing `janim-1.0.4/janim/gui/fixed_ratio_widget.py` & `janim-1.1.0/janim/gui/fixed_ratio_widget.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-
-from PySide6.QtCore import QSize
-from PySide6.QtGui import QResizeEvent
-from PySide6.QtWidgets import QWidget
-
-
-class FixedRatioWidget(QWidget):
-    '''
-    使得传入的 ``inside`` 控件可以以固定比例塞在该控件中
-    '''
-    def __init__(self, inside: QWidget, src_size: tuple[float, float], parent: QWidget | None = None) -> None:
-        super().__init__(parent)
-        self.inside = inside
-        self.inside.setParent(self)
-        self.src_size = src_size
-
-    def set_src_size(self, size: tuple[float, float]) -> None:
-        self.src_size = size
-        self.update_inner_size(self.size())
-
-    def update_inner_size(self, wnd_size: QSize) -> None:
-        wnd_width, wnd_height = wnd_size.toTuple()
-        w, h = get_proportional_scale_size(*self.src_size, wnd_width, wnd_height)
-        self.inside.setGeometry(
-            (wnd_width - w) // 2,
-            (wnd_height - h) // 2,
-            w, h
-        )
-
-    def resizeEvent(self, event: QResizeEvent) -> None:
-        super().resizeEvent(event)
-        self.update_inner_size(event.size())
-
-
-def get_proportional_scale_size(src_width, src_height, tg_width, tg_height):
-    '''
-    根据 ``(tg_width, tg_height)`` 的目标大小信息，
-    得到 ``(src_width, src_height)`` 在进行等比缩放后能塞进目标区域的最大大小
-    '''
-    factor1 = tg_width / src_width
-    factor2 = tg_height / src_height
-    factor = min(factor1, factor2)
-    return src_width * factor, src_height * factor
+
+from PySide6.QtCore import QSize
+from PySide6.QtGui import QResizeEvent
+from PySide6.QtWidgets import QWidget
+
+
+class FixedRatioWidget(QWidget):
+    '''
+    使得传入的 ``inside`` 控件可以以固定比例塞在该控件中
+    '''
+    def __init__(self, inside: QWidget, src_size: tuple[float, float], parent: QWidget | None = None) -> None:
+        super().__init__(parent)
+        self.inside = inside
+        self.inside.setParent(self)
+        self.src_size = src_size
+
+    def set_src_size(self, size: tuple[float, float]) -> None:
+        self.src_size = size
+        self.update_inner_size(self.size())
+
+    def update_inner_size(self, wnd_size: QSize) -> None:
+        wnd_width, wnd_height = wnd_size.toTuple()
+        w, h = get_proportional_scale_size(*self.src_size, wnd_width, wnd_height)
+        self.inside.setGeometry(
+            (wnd_width - w) // 2,
+            (wnd_height - h) // 2,
+            w, h
+        )
+
+    def resizeEvent(self, event: QResizeEvent) -> None:
+        super().resizeEvent(event)
+        self.update_inner_size(event.size())
+
+
+def get_proportional_scale_size(src_width, src_height, tg_width, tg_height):
+    '''
+    根据 ``(tg_width, tg_height)`` 的目标大小信息，
+    得到 ``(src_width, src_height)`` 在进行等比缩放后能塞进目标区域的最大大小
+    '''
+    factor1 = tg_width / src_width
+    factor2 = tg_height / src_height
+    factor = min(factor1, factor2)
+    return src_width * factor, src_height * factor
```

### Comparing `janim-1.0.4/janim/gui/glwidget.py` & `janim-1.1.0/janim/gui/glwidget.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-
-import moderngl as mgl
-from PySide6.QtCore import Signal
-from PySide6.QtOpenGLWidgets import QOpenGLWidget
-from PySide6.QtWidgets import QWidget
-
-from janim.anims.timeline import TimelineAnim
-
-
-class GLWidget(QOpenGLWidget):
-    '''
-    窗口中央的渲染界面
-    '''
-    rendered = Signal()
-
-    def __init__(self, anim: TimelineAnim, parent: QWidget | None = None) -> None:
-        super().__init__(parent)
-        self.anim = anim
-        self.needs_update_clear_color = False
-
-    def set_time(self, time: float) -> None:
-        self.anim.anim_on(time)
-        self.update()
-
-    def initializeGL(self) -> None:
-        self.ctx = mgl.create_context()
-        self.ctx.enable(mgl.BLEND)
-        self.ctx.blend_func = (
-            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
-            mgl.ONE, mgl.ONE
-        )
-        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
-
-        self.qfuncs = self.context().functions()
-        self.update_clear_color()
-
-    def update_clear_color(self) -> None:
-        self.needs_update_clear_color = True
-
-    def paintGL(self) -> None:
-        if self.needs_update_clear_color:
-            self.qfuncs.glClearColor(*self.anim.cfg.background_color.rgb, 0.)
-            self.needs_update_clear_color = False
-        self.qfuncs.glClear(0x00004000 | 0x00000100)    # GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT
-        self.anim.render_all(self.ctx)
-        self.rendered.emit()
+
+import moderngl as mgl
+from PySide6.QtCore import Signal
+from PySide6.QtOpenGLWidgets import QOpenGLWidget
+from PySide6.QtWidgets import QWidget
+
+from janim.anims.timeline import TimelineAnim
+
+
+class GLWidget(QOpenGLWidget):
+    '''
+    窗口中央的渲染界面
+    '''
+    rendered = Signal()
+
+    def __init__(self, anim: TimelineAnim, parent: QWidget | None = None) -> None:
+        super().__init__(parent)
+        self.anim = anim
+        self.needs_update_clear_color = False
+
+    def set_time(self, time: float) -> None:
+        self.anim.anim_on(time)
+        self.update()
+
+    def initializeGL(self) -> None:
+        self.ctx = mgl.create_context()
+        self.ctx.enable(mgl.BLEND)
+        self.ctx.blend_func = (
+            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+            mgl.ONE, mgl.ONE
+        )
+        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
+
+        self.qfuncs = self.context().functions()
+        self.update_clear_color()
+
+    def update_clear_color(self) -> None:
+        self.needs_update_clear_color = True
+
+    def paintGL(self) -> None:
+        if self.needs_update_clear_color:
+            self.qfuncs.glClearColor(*self.anim.cfg.background_color.rgb, 0.)
+            self.needs_update_clear_color = False
+        self.qfuncs.glClear(0x00004000 | 0x00000100)    # GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT
+        self.anim.render_all(self.ctx)
+        self.rendered.emit()
```

### Comparing `janim-1.0.4/janim/gui/richtext_editor.py` & `janim-1.1.0/janim/gui/richtext_editor.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-
-import re
-
-from bs4 import BeautifulSoup, Tag
-from PySide6.QtCore import QMimeData, Signal
-from PySide6.QtGui import QColor, QSyntaxHighlighter
-from PySide6.QtWidgets import (QCheckBox, QHBoxLayout, QPlainTextEdit,
-                               QVBoxLayout, QWidget)
-
-
-class RichTextEditor(QWidget):
-    def __init__(self, parent: QWidget | None = None) -> None:
-        super().__init__(parent)
-
-        self.setup_ui()
-        self.resize(600, 400)
-        self.check_box_wordwrap.setChecked(True)
-
-    def setup_ui(self):
-        self.check_box_wordwrap = QCheckBox('自动换行')
-        self.check_box_wordwrap.stateChanged.connect(
-            lambda state: self.editor.setLineWrapMode(RichTextEdit.LineWrapMode.WidgetWidth
-                                                      if state
-                                                      else RichTextEdit.LineWrapMode.NoWrap)
-        )
-
-        self.check_box_html = QCheckBox('粘贴时识别富文本格式')
-        self.check_box_html.stateChanged.connect(self.check_box_html_state_changed)
-
-        self.editor = RichTextEdit()
-        self.editor.html_inserted.connect(lambda: self.check_box_html.setChecked(False))
-
-        self.hlayout = QHBoxLayout()
-        self.hlayout.addStretch()
-        self.hlayout.addWidget(self.check_box_wordwrap)
-        self.hlayout.addWidget(self.check_box_html)
-
-        self.vlayout = QVBoxLayout()
-        self.vlayout.addLayout(self.hlayout)
-        self.vlayout.addWidget(self.editor)
-
-        self.setLayout(self.vlayout)
-
-    def check_box_html_state_changed(self, state: bool) -> None:
-        self.editor.convert_html = state
-
-
-class RichTextEdit(QPlainTextEdit):
-    html_inserted = Signal()
-
-    def __init__(self, parent: QWidget | None = None):
-        super().__init__(parent)
-
-        font = self.font()
-        font.setFamily('Consolas')
-        font.setPointSize(10)
-        self.setFont(font)
-
-        self.highlighter = RichTextHighlighter(self.document())
-
-        self.resize(600, 400)
-        self.setWindowTitle('RichText Editor')
-
-        self.convert_html = False
-
-    def insertFromMimeData(self, source: QMimeData) -> None:
-        if self.convert_html and source.hasHtml():
-            self.insertPlainText(self.html2richtext(source.html()))
-            self.html_inserted.emit()
-        else:
-            self.insertPlainText(source.text())
-
-    @staticmethod
-    def html2richtext(html: str) -> str:
-        soup = BeautifulSoup(html, 'html.parser')
-        return RichTextEdit.parse_node(soup.find('html').find('body'))
-
-    @staticmethod
-    def parse_node(node: Tag) -> str:
-        ret = []
-        has_div = False
-        for child in node.children:
-            if not child:
-                continue
-
-            match child.name:
-                case 'div':
-                    ret.append(RichTextEdit.parse_node(child))
-                    has_div = True
-                case 'span':
-                    ret.append(RichTextEdit.parse_span(child))
-                case 'br':
-                    ret.append('')
-                case _:
-                    if child.text:
-                        ret.append(child.text)
-
-        return ('\n' if has_div else '').join(ret)
-
-    @staticmethod
-    def parse_span(span: Tag) -> str:
-        if span.text.isspace():
-            style = None
-        else:
-            style = RichTextEdit.parse_style(span.get('style', ''))
-
-        return (
-            f'<fc {RichTextEdit.parse_color(style['color'])}>{span.text}</fc>'
-            if style is not None and 'color' in style
-            else span.text
-        )
-
-    @staticmethod
-    def parse_color(color: str) -> str:
-        if color.startswith('#'):
-            return color
-
-        if color.startswith('rgb(') and color.endswith(')'):
-            rgb = color.lstrip('rgb(').rstrip(')').split(',')
-            return ' '.join([
-                str(round(float(v) / 255, 2))
-                for v in rgb
-            ])
-
-        if color.startswith('rgba(') and color.endswith(')'):
-            rgba = color.lstrip('rgba(').rstrip(')').split(',')
-            return ' '.join([
-                str(round(float(v) / 255, 2))
-                for v in rgba[:3]
-            ]) + f' {rgba[3]}'
-
-        return color
-
-    @staticmethod
-    def parse_style(style: str) -> dict[str, str]:
-        ret = {}
-        for pair in style.split(';'):
-            split = pair.split(':')
-            if len(split) != 2:
-                continue
-            key, value = split
-            ret[key.strip()] = value.strip()
-        return ret
-
-
-class RichTextHighlighter(QSyntaxHighlighter):
-    regex = re.compile(r'(<+)/?[^<]*?>')
-    color = QColor(86, 156, 214)
-
-    def highlightBlock(self, text: str) -> None:
-        iter = re.finditer(self.regex, text)
-        for match in iter:
-            match: re.Match
-            start, end = match.span()
-            left = match.group(1)
-
-            left_cnt = len(left)
-
-            if left_cnt % 2 == 0:
-                continue
-            else:
-                start += left_cnt // 2
-                self.setFormat(start, end - start, self.color)
+
+import re
+
+from bs4 import BeautifulSoup, Tag
+from PySide6.QtCore import QMimeData, Signal
+from PySide6.QtGui import QColor, QSyntaxHighlighter
+from PySide6.QtWidgets import (QCheckBox, QHBoxLayout, QPlainTextEdit,
+                               QVBoxLayout, QWidget)
+
+
+class RichTextEditor(QWidget):
+    def __init__(self, parent: QWidget | None = None) -> None:
+        super().__init__(parent)
+
+        self.setup_ui()
+        self.resize(600, 400)
+        self.check_box_wordwrap.setChecked(True)
+
+    def setup_ui(self):
+        self.check_box_wordwrap = QCheckBox('自动换行')
+        self.check_box_wordwrap.stateChanged.connect(
+            lambda state: self.editor.setLineWrapMode(RichTextEdit.LineWrapMode.WidgetWidth
+                                                      if state
+                                                      else RichTextEdit.LineWrapMode.NoWrap)
+        )
+
+        self.check_box_html = QCheckBox('粘贴时识别富文本格式')
+        self.check_box_html.stateChanged.connect(self.check_box_html_state_changed)
+
+        self.editor = RichTextEdit()
+        self.editor.html_inserted.connect(lambda: self.check_box_html.setChecked(False))
+
+        self.hlayout = QHBoxLayout()
+        self.hlayout.addStretch()
+        self.hlayout.addWidget(self.check_box_wordwrap)
+        self.hlayout.addWidget(self.check_box_html)
+
+        self.vlayout = QVBoxLayout()
+        self.vlayout.addLayout(self.hlayout)
+        self.vlayout.addWidget(self.editor)
+
+        self.setLayout(self.vlayout)
+
+    def check_box_html_state_changed(self, state: bool) -> None:
+        self.editor.convert_html = state
+
+
+class RichTextEdit(QPlainTextEdit):
+    html_inserted = Signal()
+
+    def __init__(self, parent: QWidget | None = None):
+        super().__init__(parent)
+
+        font = self.font()
+        font.setFamily('Consolas')
+        font.setPointSize(10)
+        self.setFont(font)
+
+        self.highlighter = RichTextHighlighter(self.document())
+
+        self.resize(600, 400)
+        self.setWindowTitle('RichText Editor')
+
+        self.convert_html = False
+
+    def insertFromMimeData(self, source: QMimeData) -> None:
+        if self.convert_html and source.hasHtml():
+            self.insertPlainText(self.html2richtext(source.html()))
+            self.html_inserted.emit()
+        else:
+            self.insertPlainText(source.text())
+
+    @staticmethod
+    def html2richtext(html: str) -> str:
+        soup = BeautifulSoup(html, 'html.parser')
+        return RichTextEdit.parse_node(soup.find('html').find('body'))
+
+    @staticmethod
+    def parse_node(node: Tag) -> str:
+        ret = []
+        has_div = False
+        for child in node.children:
+            if not child:
+                continue
+
+            match child.name:
+                case 'div':
+                    ret.append(RichTextEdit.parse_node(child))
+                    has_div = True
+                case 'span':
+                    ret.append(RichTextEdit.parse_span(child))
+                case 'br':
+                    ret.append('')
+                case _:
+                    if child.text:
+                        ret.append(child.text)
+
+        return ('\n' if has_div else '').join(ret)
+
+    @staticmethod
+    def parse_span(span: Tag) -> str:
+        if span.text.isspace():
+            style = None
+        else:
+            style = RichTextEdit.parse_style(span.get('style', ''))
+
+        return (
+            f'<fc {RichTextEdit.parse_color(style['color'])}>{span.text}</fc>'
+            if style is not None and 'color' in style
+            else span.text
+        )
+
+    @staticmethod
+    def parse_color(color: str) -> str:
+        if color.startswith('#'):
+            return color
+
+        if color.startswith('rgb(') and color.endswith(')'):
+            rgb = color.lstrip('rgb(').rstrip(')').split(',')
+            return ' '.join([
+                str(round(float(v) / 255, 2))
+                for v in rgb
+            ])
+
+        if color.startswith('rgba(') and color.endswith(')'):
+            rgba = color.lstrip('rgba(').rstrip(')').split(',')
+            return ' '.join([
+                str(round(float(v) / 255, 2))
+                for v in rgba[:3]
+            ]) + f' {rgba[3]}'
+
+        return color
+
+    @staticmethod
+    def parse_style(style: str) -> dict[str, str]:
+        ret = {}
+        for pair in style.split(';'):
+            split = pair.split(':')
+            if len(split) != 2:
+                continue
+            key, value = split
+            ret[key.strip()] = value.strip()
+        return ret
+
+
+class RichTextHighlighter(QSyntaxHighlighter):
+    regex = re.compile(r'(<+)/?[^<]*?>')
+    color = QColor(86, 156, 214)
+
+    def highlightBlock(self, text: str) -> None:
+        iter = re.finditer(self.regex, text)
+        for match in iter:
+            match: re.Match
+            start, end = match.span()
+            left = match.group(1)
+
+            left_cnt = len(left)
+
+            if left_cnt % 2 == 0:
+                continue
+            else:
+                start += left_cnt // 2
+                self.setFormat(start, end - start, self.color)
```

### Comparing `janim-1.0.4/janim/gui/selector.py` & `janim-1.1.0/janim/gui/selector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,521 +1,508 @@
-00000000: 0d0a 6672 6f6d 2064 6174 6163 6c61 7373  ..from dataclass
-00000010: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00000020: 6173 730d 0a66 726f 6d20 7479 7069 6e67  ass..from typing
-00000030: 2069 6d70 6f72 7420 5459 5045 5f43 4845   import TYPE_CHE
-00000040: 434b 494e 470d 0a0d 0a66 726f 6d20 5079  CKING....from Py
-00000050: 5369 6465 362e 5174 436f 7265 2069 6d70  Side6.QtCore imp
-00000060: 6f72 7420 5145 7665 6e74 2c20 514f 626a  ort QEvent, QObj
-00000070: 6563 742c 2051 506f 696e 7446 2c20 5152  ect, QPointF, QR
-00000080: 6563 7446 2c20 5174 0d0a 6672 6f6d 2050  ectF, Qt..from P
-00000090: 7953 6964 6536 2e51 7447 7569 2069 6d70  ySide6.QtGui imp
-000000a0: 6f72 7420 5143 6f6c 6f72 2c20 514d 6f75  ort QColor, QMou
-000000b0: 7365 4576 656e 742c 2051 5061 696e 7465  seEvent, QPainte
-000000c0: 722c 2051 5061 696e 7445 7665 6e74 0d0a  r, QPaintEvent..
-000000d0: 0d0a 6672 6f6d 206a 616e 696d 2e61 6e69  ..from janim.ani
-000000e0: 6d73 2e64 6973 706c 6179 2069 6d70 6f72  ms.display impor
-000000f0: 7420 4469 7370 6c61 790d 0a66 726f 6d20  t Display..from 
-00000100: 6a61 6e69 6d2e 6974 656d 732e 6974 656d  janim.items.item
-00000110: 2069 6d70 6f72 7420 4974 656d 0d0a 6672   import Item..fr
-00000120: 6f6d 206a 616e 696d 2e69 7465 6d73 2e70  om janim.items.p
-00000130: 6f69 6e74 7320 696d 706f 7274 2050 6f69  oints import Poi
-00000140: 6e74 730d 0a0d 0a69 6620 5459 5045 5f43  nts....if TYPE_C
-00000150: 4845 434b 494e 473a 0d0a 2020 2020 6672  HECKING:..    fr
-00000160: 6f6d 206a 616e 696d 2e67 7569 2e61 6e69  om janim.gui.ani
-00000170: 6d5f 7669 6577 6572 2069 6d70 6f72 7420  m_viewer import 
-00000180: 416e 696d 5669 6577 6572 0d0a 0d0a 0d0a  AnimViewer......
-00000190: 636c 6173 7320 5365 6c65 6374 6f72 2851  class Selector(Q
-000001a0: 4f62 6a65 6374 293a 0d0a 2020 2020 2727  Object):..    ''
-000001b0: 270d 0a20 2020 20e5 ad90 e789 a9e4 bbb6  '..    .........
-000001c0: e980 89e6 8ba9 e5b7 a5e5 85b7 0d0a 2020  ..............  
-000001d0: 2020 2727 270d 0a20 2020 2040 6461 7461    '''..    @data
-000001e0: 636c 6173 730d 0a20 2020 2063 6c61 7373  class..    class
-000001f0: 2053 656c 6563 7465 6449 7465 6d3a 0d0a   SelectedItem:..
-00000200: 2020 2020 2020 2020 6974 656d 3a20 4974          item: It
-00000210: 656d 0d0a 2020 2020 2020 2020 6d69 6e5f  em..        min_
-00000220: 676c 783a 2066 6c6f 6174 0d0a 2020 2020  glx: float..    
-00000230: 2020 2020 6d69 6e5f 676c 793a 2066 6c6f      min_gly: flo
-00000240: 6174 0d0a 2020 2020 2020 2020 6d61 785f  at..        max_
-00000250: 676c 783a 2066 6c6f 6174 0d0a 2020 2020  glx: float..    
-00000260: 2020 2020 6d61 785f 676c 793a 2066 6c6f      max_gly: flo
-00000270: 6174 0d0a 0d0a 2020 2020 6465 6620 5f5f  at....    def __
-00000280: 696e 6974 5f5f 2873 656c 662c 2070 6172  init__(self, par
-00000290: 656e 743a 2027 416e 696d 5669 6577 6572  ent: 'AnimViewer
-000002a0: 2729 202d 3e20 4e6f 6e65 3a0d 0a20 2020  ') -> None:..   
-000002b0: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-000002c0: 6e69 745f 5f28 7061 7265 6e74 290d 0a20  nit__(parent).. 
-000002d0: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
-000002e0: 6572 203d 2070 6172 656e 740d 0a0d 0a20  er = parent.... 
-000002f0: 2020 2020 2020 2073 656c 662e 7669 6577         self.view
-00000300: 6572 2e67 6c77 2e69 6e73 7461 6c6c 4576  er.glw.installEv
-00000310: 656e 7446 696c 7465 7228 7365 6c66 290d  entFilter(self).
-00000320: 0a20 2020 2020 2020 2073 656c 662e 7669  .        self.vi
-00000330: 6577 6572 2e6f 7665 726c 6179 2e69 6e73  ewer.overlay.ins
-00000340: 7461 6c6c 4576 656e 7446 696c 7465 7228  tallEventFilter(
-00000350: 7365 6c66 290d 0a0d 0a20 2020 2020 2020  self)....       
-00000360: 2073 656c 662e 636c 6561 7228 290d 0a0d   self.clear()...
-00000370: 0a20 2020 2064 6566 2063 6c65 6172 2873  .    def clear(s
-00000380: 656c 6629 202d 3e20 4e6f 6e65 3a0d 0a20  elf) -> None:.. 
-00000390: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
-000003a0: 656e 743a 2053 656c 6563 746f 722e 5365  ent: Selector.Se
-000003b0: 6c65 6374 6564 4974 656d 207c 204e 6f6e  lectedItem | Non
-000003c0: 6520 3d20 4e6f 6e65 0d0a 2020 2020 2020  e = None..      
-000003d0: 2020 7365 6c66 2e63 6869 6c64 7265 6e3a    self.children:
-000003e0: 206c 6973 745b 5365 6c65 6374 6f72 2e53   list[Selector.S
-000003f0: 656c 6563 7465 6449 7465 6d5d 203d 205b  electedItem] = [
-00000400: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
-00000410: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
-00000420: 6e3a 206c 6973 745b 5365 6c65 6374 6f72  n: list[Selector
-00000430: 2e53 656c 6563 7465 6449 7465 6d5d 203d  .SelectedItem] =
-00000440: 205b 5d0d 0a20 2020 2020 2020 2073 656c   []..        sel
-00000450: 662e 7669 6577 6572 2e6f 7665 726c 6179  f.viewer.overlay
-00000460: 2e75 7064 6174 6528 290d 0a0d 0a20 2020  .update()....   
-00000470: 2064 6566 2067 6c78 5f74 6f5f 6f76 6572   def glx_to_over
-00000480: 6c61 795f 7828 7365 6c66 2c20 676c 783a  lay_x(self, glx:
-00000490: 2066 6c6f 6174 2920 2d3e 2066 6c6f 6174   float) -> float
-000004a0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-000004b0: 6e20 2867 6c78 202b 2031 2920 2f20 3220  n (glx + 1) / 2 
-000004c0: 2a20 7365 6c66 2e76 6965 7765 722e 6f76  * self.viewer.ov
-000004d0: 6572 6c61 792e 7769 6474 6828 290d 0a0d  erlay.width()...
-000004e0: 0a20 2020 2064 6566 2067 6c79 5f74 6f5f  .    def gly_to_
-000004f0: 6f76 6572 6c61 795f 7928 7365 6c66 2c20  overlay_y(self, 
-00000500: 676c 793a 2066 6c6f 6174 2920 2d3e 2066  gly: float) -> f
-00000510: 6c6f 6174 3a0d 0a20 2020 2020 2020 2072  loat:..        r
-00000520: 6574 7572 6e20 282d 676c 7920 2b20 3129  eturn (-gly + 1)
-00000530: 202f 2032 202a 2073 656c 662e 7669 6577   / 2 * self.view
-00000540: 6572 2e6f 7665 726c 6179 2e68 6569 6768  er.overlay.heigh
-00000550: 7428 290d 0a0d 0a20 2020 2064 6566 2065  t()....    def e
-00000560: 7665 6e74 4669 6c74 6572 2873 656c 662c  ventFilter(self,
-00000570: 2077 6174 6368 6564 3a20 514f 626a 6563   watched: QObjec
-00000580: 742c 2065 7665 6e74 3a20 5145 7665 6e74  t, event: QEvent
-00000590: 2920 2d3e 2062 6f6f 6c3a 0d0a 2020 2020  ) -> bool:..    
-000005a0: 2020 2020 6966 2077 6174 6368 6564 2069      if watched i
-000005b0: 7320 7365 6c66 2e76 6965 7765 722e 676c  s self.viewer.gl
-000005c0: 773a 0d0a 2020 2020 2020 2020 2020 2020  w:..            
-000005d0: 6966 2065 7665 6e74 2e74 7970 6528 2920  if event.type() 
-000005e0: 696e 2028 5145 7665 6e74 2e54 7970 652e  in (QEvent.Type.
-000005f0: 4d6f 7573 6542 7574 746f 6e50 7265 7373  MouseButtonPress
-00000600: 2c20 5145 7665 6e74 2e54 7970 652e 4d6f  , QEvent.Type.Mo
-00000610: 7573 6542 7574 746f 6e44 626c 436c 6963  useButtonDblClic
-00000620: 6b29 3a0d 0a20 2020 2020 2020 2020 2020  k):..           
-00000630: 2020 2020 2073 656c 662e 6f6e 5f67 6c77       self.on_glw
-00000640: 5f6d 6f75 7365 5f70 7265 7373 2865 7665  _mouse_press(eve
-00000650: 6e74 290d 0a20 2020 2020 2020 2020 2020  nt)..           
-00000660: 2069 6620 6576 656e 742e 7479 7065 2829   if event.type()
-00000670: 203d 3d20 5145 7665 6e74 2e54 7970 652e   == QEvent.Type.
-00000680: 4d6f 7573 654d 6f76 653a 0d0a 2020 2020  MouseMove:..    
-00000690: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000006a0: 2e6f 6e5f 676c 775f 6d6f 7573 655f 6d6f  .on_glw_mouse_mo
-000006b0: 7665 2865 7665 6e74 290d 0a0d 0a20 2020  ve(event)....   
-000006c0: 2020 2020 2069 6620 7761 7463 6865 6420       if watched 
-000006d0: 6973 2073 656c 662e 7669 6577 6572 2e6f  is self.viewer.o
-000006e0: 7665 726c 6179 3a0d 0a20 2020 2020 2020  verlay:..       
-000006f0: 2020 2020 2069 6620 6576 656e 742e 7479       if event.ty
-00000700: 7065 2829 203d 3d20 5145 7665 6e74 2e54  pe() == QEvent.T
-00000710: 7970 652e 5061 696e 743a 0d0a 2020 2020  ype.Paint:..    
-00000720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000730: 2e6f 6e5f 6f76 6572 6c61 795f 7061 696e  .on_overlay_pain
-00000740: 7428 6576 656e 7429 0d0a 0d0a 2020 2020  t(event)....    
-00000750: 2020 2020 7265 7475 726e 2073 7570 6572      return super
-00000760: 2829 2e65 7665 6e74 4669 6c74 6572 2877  ().eventFilter(w
-00000770: 6174 6368 6564 2c20 6576 656e 7429 0d0a  atched, event)..
-00000780: 0d0a 2020 2020 6465 6620 6f6e 5f67 6c77  ..    def on_glw
-00000790: 5f6d 6f75 7365 5f70 7265 7373 2873 656c  _mouse_press(sel
-000007a0: 662c 2065 7665 6e74 3a20 514d 6f75 7365  f, event: QMouse
-000007b0: 4576 656e 7429 202d 3e20 4e6f 6e65 3a0d  Event) -> None:.
-000007c0: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-000007d0: 742e 6d6f 6469 6669 6572 7328 2920 2620  t.modifiers() & 
-000007e0: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
-000007f0: 6965 722e 436f 6e74 726f 6c4d 6f64 6966  ier.ControlModif
-00000800: 6965 723a 0d0a 2020 2020 2020 2020 2020  ier:..          
-00000810: 2020 6d61 7463 6820 6576 656e 742e 6275    match event.bu
-00000820: 7474 6f6e 2829 3a0d 0a20 2020 2020 2020  tton():..       
-00000830: 2020 2020 2020 2020 2063 6173 6520 5174           case Qt
-00000840: 2e4d 6f75 7365 4275 7474 6f6e 2e4c 6566  .MouseButton.Lef
-00000850: 7442 7574 746f 6e3a 0d0a 2020 2020 2020  tButton:..      
-00000860: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000870: 6c66 2e73 656c 6563 745f 7061 7265 6e74  lf.select_parent
-00000880: 5f69 7465 6d28 6576 656e 7429 0d0a 2020  _item(event)..  
-00000890: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000008a0: 7365 2051 742e 4d6f 7573 6542 7574 746f  se Qt.MouseButto
-000008b0: 6e2e 5269 6768 7442 7574 746f 6e3a 0d0a  n.RightButton:..
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2020 7365 6c66 2e64 656c 6574 654c      self.deleteL
-000008e0: 6174 6572 2829 0d0a 2020 2020 2020 2020  ater()..        
-000008f0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00000900: 2020 206d 6174 6368 2065 7665 6e74 2e62     match event.b
-00000910: 7574 746f 6e28 293a 0d0a 2020 2020 2020  utton():..      
-00000920: 2020 2020 2020 2020 2020 6361 7365 2051            case Q
-00000930: 742e 4d6f 7573 6542 7574 746f 6e2e 4c65  t.MouseButton.Le
-00000940: 6674 4275 7474 6f6e 3a0d 0a20 2020 2020  ftButton:..     
-00000950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000960: 656c 662e 7365 6c65 6374 5f63 6869 6c64  elf.select_child
-00000970: 5f69 7465 6d28 6576 656e 7429 0d0a 2020  _item(event)..  
-00000980: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00000990: 7365 2051 742e 4d6f 7573 6542 7574 746f  se Qt.MouseButto
-000009a0: 6e2e 5269 6768 7442 7574 746f 6e3a 0d0a  n.RightButton:..
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 7365 6c66 2e72 656d 6f76 655f      self.remove_
-000009d0: 6368 696c 645f 6974 656d 2865 7665 6e74  child_item(event
-000009e0: 290d 0a0d 0a20 2020 2020 2020 2073 656c  )....        sel
-000009f0: 662e 7669 6577 6572 2e6f 7665 726c 6179  f.viewer.overlay
-00000a00: 2e75 7064 6174 6528 290d 0a0d 0a20 2020  .update()....   
-00000a10: 2064 6566 206f 6e5f 676c 775f 6d6f 7573   def on_glw_mous
-00000a20: 655f 6d6f 7665 2873 656c 662c 2065 7665  e_move(self, eve
-00000a30: 6e74 3a20 514d 6f75 7365 4576 656e 7429  nt: QMouseEvent)
-00000a40: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-00000a50: 2020 2069 6620 6e6f 7420 6576 656e 742e     if not event.
-00000a60: 6d6f 6469 6669 6572 7328 2920 2620 5174  modifiers() & Qt
-00000a70: 2e4b 6579 626f 6172 644d 6f64 6966 6965  .KeyboardModifie
-00000a80: 722e 436f 6e74 726f 6c4d 6f64 6966 6965  r.ControlModifie
-00000a90: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00000aa0: 6d61 7463 6820 6576 656e 742e 6275 7474  match event.butt
-00000ab0: 6f6e 7328 293a 0d0a 2020 2020 2020 2020  ons():..        
-00000ac0: 2020 2020 2020 2020 6361 7365 2051 742e          case Qt.
-00000ad0: 4d6f 7573 6542 7574 746f 6e2e 4c65 6674  MouseButton.Left
-00000ae0: 4275 7474 6f6e 3a0d 0a20 2020 2020 2020  Button:..       
-00000af0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00000b00: 662e 7365 6c65 6374 5f63 6869 6c64 5f69  f.select_child_i
-00000b10: 7465 6d28 6576 656e 7429 0d0a 2020 2020  tem(event)..    
-00000b20: 2020 2020 2020 2020 2020 2020 6361 7365              case
-00000b30: 2051 742e 4d6f 7573 6542 7574 746f 6e2e   Qt.MouseButton.
-00000b40: 5269 6768 7442 7574 746f 6e3a 0d0a 2020  RightButton:..  
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 7365 6c66 2e72 656d 6f76 655f 6368    self.remove_ch
-00000b70: 696c 645f 6974 656d 2865 7665 6e74 290d  ild_item(event).
-00000b80: 0a0d 0a20 2020 2020 2020 2020 2020 2073  ...            s
-00000b90: 656c 662e 7669 6577 6572 2e6f 7665 726c  elf.viewer.overl
-00000ba0: 6179 2e75 7064 6174 6528 290d 0a0d 0a20  ay.update().... 
-00000bb0: 2020 2064 6566 2073 656c 6563 745f 7061     def select_pa
-00000bc0: 7265 6e74 5f69 7465 6d28 7365 6c66 2c20  rent_item(self, 
-00000bd0: 6576 656e 743a 2051 4d6f 7573 6545 7665  event: QMouseEve
-00000be0: 6e74 2920 2d3e 204e 6f6e 653a 0d0a 2020  nt) -> None:..  
-00000bf0: 2020 2020 2020 7365 6c66 2e63 6869 6c64        self.child
-00000c00: 7265 6e2e 636c 6561 7228 290d 0a20 2020  ren.clear()..   
-00000c10: 2020 2020 2073 656c 662e 7365 6c65 6374       self.select
-00000c20: 6564 5f63 6869 6c64 7265 6e2e 636c 6561  ed_children.clea
-00000c30: 7228 290d 0a0d 0a20 2020 2020 2020 2078  r()....        x
-00000c40: 2c20 7920 3d20 6576 656e 742e 706f 7369  , y = event.posi
-00000c50: 7469 6f6e 2829 2e74 6f54 7570 6c65 2829  tion().toTuple()
-00000c60: 0d0a 2020 2020 2020 2020 676c 7820 3d20  ..        glx = 
-00000c70: 7820 2f20 7365 6c66 2e76 6965 7765 722e  x / self.viewer.
-00000c80: 676c 772e 7769 6474 6828 2920 2a20 3220  glw.width() * 2 
-00000c90: 2d20 310d 0a20 2020 2020 2020 2067 6c79  - 1..        gly
-00000ca0: 203d 2079 202f 2073 656c 662e 7669 6577   = y / self.view
-00000cb0: 6572 2e67 6c77 2e68 6569 6768 7428 2920  er.glw.height() 
-00000cc0: 2a20 2d32 202b 2031 0d0a 0d0a 2020 2020  * -2 + 1....    
-00000cd0: 2020 2020 616e 696d 203d 2073 656c 662e      anim = self.
-00000ce0: 7669 6577 6572 2e61 6e69 6d0d 0a20 2020  viewer.anim..   
-00000cf0: 2020 2020 2067 6c6f 6261 6c5f 7420 3d20       global_t = 
-00000d00: 616e 696d 2e5f 7469 6d65 0d0a 2020 2020  anim._time..    
-00000d10: 2020 2020 6361 6d65 7261 5f69 6e66 6f20      camera_info 
-00000d20: 3d20 616e 696d 2e74 696d 656c 696e 652e  = anim.timeline.
-00000d30: 6361 6d65 7261 2e63 7572 7265 6e74 2861  camera.current(a
-00000d40: 735f 7469 6d65 3d67 6c6f 6261 6c5f 7429  s_time=global_t)
-00000d50: 2e70 6f69 6e74 732e 696e 666f 0d0a 0d0a  .points.info....
-00000d60: 2020 2020 2020 2020 666f 756e 643a 206c          found: l
-00000d70: 6973 745b 5365 6c65 6374 6f72 2e53 656c  ist[Selector.Sel
-00000d80: 6563 7465 6449 7465 6d5d 203d 205b 5d0d  ectedItem] = [].
-00000d90: 0a0d 0a20 2020 2020 2020 2066 6f72 2064  ...        for d
-00000da0: 6973 706c 6179 2069 6e20 616e 696d 2e64  isplay in anim.d
-00000db0: 6973 706c 6179 5f61 6e69 6d2e 616e 696d  isplay_anim.anim
-00000dc0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000dd0: 6469 7370 6c61 793a 2044 6973 706c 6179  display: Display
-00000de0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000df0: 206e 6f74 2064 6973 706c 6179 2e67 6c6f   not display.glo
-00000e00: 6261 6c5f 7261 6e67 652e 6174 203c 3d20  bal_range.at <= 
-00000e10: 676c 6f62 616c 5f74 203c 2064 6973 706c  global_t < displ
-00000e20: 6179 2e67 6c6f 6261 6c5f 7261 6e67 652e  ay.global_range.
-00000e30: 656e 643a 0d0a 2020 2020 2020 2020 2020  end:..          
-00000e40: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00000e50: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-00000e60: 7820 3d20 6469 7370 6c61 792e 6974 656d  x = display.item
-00000e70: 2e63 7572 7265 6e74 2861 735f 7469 6d65  .current(as_time
-00000e80: 3d67 6c6f 6261 6c5f 7429 2850 6f69 6e74  =global_t)(Point
-00000e90: 7329 2e70 6f69 6e74 732e 626f 780d 0a0d  s).points.box...
-00000ea0: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
-00000eb0: 7065 6420 3d20 6361 6d65 7261 5f69 6e66  ped = camera_inf
-00000ec0: 6f2e 6d61 705f 706f 696e 7473 2862 6f78  o.map_points(box
-00000ed0: 2e67 6574 5f63 6f72 6e65 7273 2829 290d  .get_corners()).
-00000ee0: 0a20 2020 2020 2020 2020 2020 206d 696e  .            min
-00000ef0: 5f67 6c78 2c20 6d69 6e5f 676c 7920 3d20  _glx, min_gly = 
-00000f00: 6d61 7070 6564 2e6d 696e 2861 7869 733d  mapped.min(axis=
-00000f10: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-00000f20: 6d61 785f 676c 782c 206d 6178 5f67 6c79  max_glx, max_gly
-00000f30: 203d 206d 6170 7065 642e 6d61 7828 6178   = mapped.max(ax
-00000f40: 6973 3d30 290d 0a20 2020 2020 2020 2020  is=0)..         
-00000f50: 2020 2069 6620 6e6f 7420 6d69 6e5f 676c     if not min_gl
-00000f60: 7820 3c3d 2067 6c78 203c 3d20 6d61 785f  x <= glx <= max_
-00000f70: 676c 7820 6f72 206e 6f74 206d 696e 5f67  glx or not min_g
-00000f80: 6c79 203c 3d20 676c 7920 3c3d 206d 6178  ly <= gly <= max
-00000f90: 5f67 6c79 3a0d 0a20 2020 2020 2020 2020  _gly:..         
-00000fa0: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00000fb0: 0a0d 0a20 2020 2020 2020 2020 2020 2066  ...            f
-00000fc0: 6f75 6e64 2e61 7070 656e 6428 5365 6c65  ound.append(Sele
-00000fd0: 6374 6f72 2e53 656c 6563 7465 6449 7465  ctor.SelectedIte
-00000fe0: 6d28 6469 7370 6c61 792e 6974 656d 2c20  m(display.item, 
-00000ff0: 6d69 6e5f 676c 782c 206d 696e 5f67 6c79  min_glx, min_gly
-00001000: 2c20 6d61 785f 676c 782c 206d 6178 5f67  , max_glx, max_g
-00001010: 6c79 2929 0d0a 0d0a 2020 2020 2020 2020  ly))....        
-00001020: 6966 206e 6f74 2066 6f75 6e64 3a0d 0a20  if not found:.. 
-00001030: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001040: 6375 7272 656e 7420 3d20 4e6f 6e65 0d0a  current = None..
-00001050: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00001060: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00001070: 6c66 2e63 7572 7265 6e74 2069 7320 4e6f  lf.current is No
-00001080: 6e65 206f 7220 7365 6c66 2e63 7572 7265  ne or self.curre
-00001090: 6e74 206e 6f74 2069 6e20 666f 756e 643a  nt not in found:
-000010a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000010b0: 2020 7365 6c66 2e63 7572 7265 6e74 203d    self.current =
-000010c0: 2066 6f75 6e64 5b30 5d0d 0a20 2020 2020   found[0]..     
-000010d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 6964                id
-000010f0: 7820 3d20 666f 756e 642e 696e 6465 7828  x = found.index(
-00001100: 7365 6c66 2e63 7572 7265 6e74 290d 0a20  self.current).. 
-00001110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001120: 656c 662e 6375 7272 656e 7420 3d20 666f  elf.current = fo
-00001130: 756e 645b 2869 6478 202b 2031 2920 2520  und[(idx + 1) % 
-00001140: 6c65 6e28 666f 756e 6429 5d0d 0a0d 0a20  len(found)].... 
-00001150: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00001160: 7465 6d20 696e 2073 656c 662e 6375 7272  tem in self.curr
-00001170: 656e 742e 6974 656d 2e67 6574 5f63 6869  ent.item.get_chi
-00001180: 6c64 7265 6e28 293a 0d0a 2020 2020 2020  ldren():..      
-00001190: 2020 2020 2020 2020 2020 626f 7820 3d20            box = 
-000011a0: 6974 656d 2e63 7572 7265 6e74 2861 735f  item.current(as_
-000011b0: 7469 6d65 3d67 6c6f 6261 6c5f 7429 2850  time=global_t)(P
-000011c0: 6f69 6e74 7329 2e70 6f69 6e74 732e 626f  oints).points.bo
-000011d0: 780d 0a20 2020 2020 2020 2020 2020 2020  x..             
-000011e0: 2020 206d 6170 7065 6420 3d20 6361 6d65     mapped = came
-000011f0: 7261 5f69 6e66 6f2e 6d61 705f 706f 696e  ra_info.map_poin
-00001200: 7473 2862 6f78 2e67 6574 5f63 6f72 6e65  ts(box.get_corne
-00001210: 7273 2829 290d 0a20 2020 2020 2020 2020  rs())..         
-00001220: 2020 2020 2020 2073 656c 662e 6368 696c         self.chil
-00001230: 6472 656e 2e61 7070 656e 6428 5365 6c65  dren.append(Sele
-00001240: 6374 6f72 2e53 656c 6563 7465 6449 7465  ctor.SelectedIte
-00001250: 6d28 6974 656d 2c20 2a6d 6170 7065 642e  m(item, *mapped.
-00001260: 6d69 6e28 6178 6973 3d30 292c 202a 6d61  min(axis=0), *ma
-00001270: 7070 6564 2e6d 6178 2861 7869 733d 3029  pped.max(axis=0)
-00001280: 2929 0d0a 0d0a 2020 2020 6465 6620 7365  ))....    def se
-00001290: 6c65 6374 5f63 6869 6c64 5f69 7465 6d28  lect_child_item(
-000012a0: 7365 6c66 2c20 6576 656e 743a 2051 4d6f  self, event: QMo
-000012b0: 7573 6545 7665 6e74 2920 2d3e 204e 6f6e  useEvent) -> Non
-000012c0: 653a 0d0a 2020 2020 2020 2020 782c 2079  e:..        x, y
-000012d0: 203d 2065 7665 6e74 2e70 6f73 6974 696f   = event.positio
-000012e0: 6e28 292e 746f 5475 706c 6528 290d 0a20  n().toTuple().. 
-000012f0: 2020 2020 2020 2067 6c78 203d 2078 202f         glx = x /
-00001300: 2073 656c 662e 7669 6577 6572 2e67 6c77   self.viewer.glw
-00001310: 2e77 6964 7468 2829 202a 2032 202d 2031  .width() * 2 - 1
-00001320: 0d0a 2020 2020 2020 2020 676c 7920 3d20  ..        gly = 
-00001330: 7920 2f20 7365 6c66 2e76 6965 7765 722e  y / self.viewer.
-00001340: 676c 772e 6865 6967 6874 2829 202a 202d  glw.height() * -
-00001350: 3220 2b20 310d 0a0d 0a20 2020 2020 2020  2 + 1....       
-00001360: 2066 6f72 2063 6869 6c64 2069 6e20 7365   for child in se
-00001370: 6c66 2e63 6869 6c64 7265 6e3a 0d0a 2020  lf.children:..  
-00001380: 2020 2020 2020 2020 2020 6966 2063 6869            if chi
-00001390: 6c64 2069 6e20 7365 6c66 2e73 656c 6563  ld in self.selec
-000013a0: 7465 645f 6368 696c 6472 656e 3a0d 0a20  ted_children:.. 
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000013c0: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-000013d0: 2020 2020 2069 6620 6e6f 7420 6368 696c       if not chil
-000013e0: 642e 6d69 6e5f 676c 7820 3c3d 2067 6c78  d.min_glx <= glx
-000013f0: 203c 3d20 6368 696c 642e 6d61 785f 676c   <= child.max_gl
-00001400: 7820 6f72 206e 6f74 2063 6869 6c64 2e6d  x or not child.m
-00001410: 696e 5f67 6c79 203c 3d20 676c 7920 3c3d  in_gly <= gly <=
-00001420: 2063 6869 6c64 2e6d 6178 5f67 6c79 3a0d   child.max_gly:.
-00001430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001440: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00001450: 2020 2020 2020 2073 656c 662e 7365 6c65         self.sele
-00001460: 6374 6564 5f63 6869 6c64 7265 6e2e 6170  cted_children.ap
-00001470: 7065 6e64 2863 6869 6c64 290d 0a0d 0a20  pend(child).... 
-00001480: 2020 2064 6566 2072 656d 6f76 655f 6368     def remove_ch
-00001490: 696c 645f 6974 656d 2873 656c 662c 2065  ild_item(self, e
-000014a0: 7665 6e74 3a20 514d 6f75 7365 4576 656e  vent: QMouseEven
-000014b0: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
-000014c0: 2020 2020 2078 2c20 7920 3d20 6576 656e       x, y = even
-000014d0: 742e 706f 7369 7469 6f6e 2829 2e74 6f54  t.position().toT
-000014e0: 7570 6c65 2829 0d0a 2020 2020 2020 2020  uple()..        
-000014f0: 676c 7820 3d20 7820 2f20 7365 6c66 2e76  glx = x / self.v
-00001500: 6965 7765 722e 676c 772e 7769 6474 6828  iewer.glw.width(
-00001510: 2920 2a20 3220 2d20 310d 0a20 2020 2020  ) * 2 - 1..     
-00001520: 2020 2067 6c79 203d 2079 202f 2073 656c     gly = y / sel
-00001530: 662e 7669 6577 6572 2e67 6c77 2e68 6569  f.viewer.glw.hei
-00001540: 6768 7428 2920 2a20 2d32 202b 2031 0d0a  ght() * -2 + 1..
-00001550: 0d0a 2020 2020 2020 2020 666f 7220 6368  ..        for ch
-00001560: 696c 6420 696e 2073 656c 662e 7365 6c65  ild in self.sele
-00001570: 6374 6564 5f63 6869 6c64 7265 6e3a 0d0a  cted_children:..
-00001580: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00001590: 6f74 2063 6869 6c64 2e6d 696e 5f67 6c78  ot child.min_glx
-000015a0: 203c 3d20 676c 7820 3c3d 2063 6869 6c64   <= glx <= child
-000015b0: 2e6d 6178 5f67 6c78 206f 7220 6e6f 7420  .max_glx or not 
-000015c0: 6368 696c 642e 6d69 6e5f 676c 7920 3c3d  child.min_gly <=
-000015d0: 2067 6c79 203c 3d20 6368 696c 642e 6d61   gly <= child.ma
-000015e0: 785f 676c 793a 0d0a 2020 2020 2020 2020  x_gly:..        
-000015f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00001600: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001610: 6c66 2e73 656c 6563 7465 645f 6368 696c  lf.selected_chil
-00001620: 6472 656e 2e72 656d 6f76 6528 6368 696c  dren.remove(chil
-00001630: 6429 0d0a 0d0a 2020 2020 6465 6620 6f6e  d)....    def on
-00001640: 5f6f 7665 726c 6179 5f70 6169 6e74 2873  _overlay_paint(s
-00001650: 656c 662c 2065 7665 6e74 3a20 5150 6169  elf, event: QPai
-00001660: 6e74 4576 656e 7429 202d 3e20 4e6f 6e65  ntEvent) -> None
-00001670: 3a0d 0a20 2020 2020 2020 2072 6563 7420  :..        rect 
-00001680: 3d20 7365 6c66 2e76 6965 7765 722e 6f76  = self.viewer.ov
-00001690: 6572 6c61 792e 7265 6374 2829 2e61 646a  erlay.rect().adj
-000016a0: 7573 7465 6428 322c 2032 2c20 2d32 2c20  usted(2, 2, -2, 
-000016b0: 2d32 290d 0a0d 0a20 2020 2020 2020 2070  -2)....        p
-000016c0: 203d 2051 5061 696e 7465 7228 7365 6c66   = QPainter(self
-000016d0: 2e76 6965 7765 722e 6f76 6572 6c61 7929  .viewer.overlay)
-000016e0: 0d0a 0d0a 2020 2020 2020 2020 7261 6e67  ....        rang
-000016f0: 6573 3a20 6c69 7374 5b74 7570 6c65 5b66  es: list[tuple[f
-00001700: 6c6f 6174 2c20 666c 6f61 745d 5d20 3d20  loat, float]] = 
-00001710: 5b5d 0d0a 2020 2020 2020 2020 6966 2073  []..        if s
-00001720: 656c 662e 7365 6c65 6374 6564 5f63 6869  elf.selected_chi
-00001730: 6c64 7265 6e3a 0d0a 2020 2020 2020 2020  ldren:..        
-00001740: 2020 2020 7261 6e67 655f 7374 6172 7420      range_start 
-00001750: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00001760: 2020 2020 7261 6e67 655f 656e 6420 3d20      range_end = 
-00001770: 4e6f 6e65 0d0a 0d0a 2020 2020 2020 2020  None....        
-00001780: 2020 2020 666f 7220 692c 2063 6869 6c64      for i, child
-00001790: 2069 6e20 656e 756d 6572 6174 6528 7365   in enumerate(se
-000017a0: 6c66 2e63 6869 6c64 7265 6e29 3a0d 0a20  lf.children):.. 
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000017c0: 6620 6368 696c 6420 696e 2073 656c 662e  f child in self.
-000017d0: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
-000017e0: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-000017f0: 2020 2020 2020 2020 6966 2072 616e 6765          if range
-00001800: 5f73 7461 7274 2069 7320 4e6f 6e65 3a0d  _start is None:.
-00001810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001820: 2020 2020 2020 2020 2072 616e 6765 5f73           range_s
-00001830: 7461 7274 203d 2069 0d0a 2020 2020 2020  tart = i..      
-00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001850: 2020 7261 6e67 655f 656e 6420 3d20 6920    range_end = i 
-00001860: 2b20 310d 0a20 2020 2020 2020 2020 2020  + 1..           
-00001870: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001880: 7469 6e75 650d 0a0d 0a20 2020 2020 2020  tinue....       
-00001890: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000018a0: 6920 3d3d 2072 616e 6765 5f65 6e64 3a0d  i == range_end:.
-000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018c0: 2020 2020 2020 2020 2072 616e 6765 5f65           range_e
-000018d0: 6e64 202b 3d20 310d 0a20 2020 2020 2020  nd += 1..       
-000018e0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000018f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00001900: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
-00001910: 6573 2e61 7070 656e 6428 2872 616e 6765  es.append((range
-00001920: 5f73 7461 7274 2c20 7261 6e67 655f 656e  _start, range_en
-00001930: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00001940: 2020 2020 2020 2020 2020 2020 2072 616e               ran
-00001950: 6765 5f73 7461 7274 203d 2069 0d0a 2020  ge_start = i..  
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001970: 2020 2020 2020 7261 6e67 655f 656e 6420        range_end 
-00001980: 3d20 6920 2b20 310d 0a20 2020 2020 2020  = i + 1..       
-00001990: 2020 2020 2072 616e 6765 732e 6170 7065       ranges.appe
-000019a0: 6e64 2828 7261 6e67 655f 7374 6172 742c  nd((range_start,
-000019b0: 2072 616e 6765 5f65 6e64 2929 0d0a 0d0a   range_end))....
-000019c0: 2020 2020 2020 2020 7478 745f 6c69 7374          txt_list
-000019d0: 203d 205b 0d0a 2020 2020 2020 2020 2020   = [..          
-000019e0: 2020 27e5 ad90 e789 a9e4 bbb6 e980 89e6    '.............
-000019f0: 8ba9 e5b7 a5e5 85b7 efbc 8843 7472 6c2b  ...........Ctrl+
-00001a00: e5b7 a6e9 94ae 3a20 e980 89e6 8ba9 e788  ......: ........
-00001a10: b6e7 89a9 e4bb b6ef bc8c e5b7 a6e9 94ae  ................
-00001a20: 3a20 e980 89e6 8ba9 e5ad 90e7 89a9 e4bb  : ..............
-00001a30: b6ef bc8c e58f b3e9 94ae 3a20 e58f 96e6  ..........: ....
-00001a40: b688 e980 89e6 8ba9 e5ad 90e7 89a9 e4bb  ................
-00001a50: b6ef bc8c 4374 726c 2be5 8fb3 e994 ae3a  ....Ctrl+......:
-00001a60: 20e9 8080 e587 baef bc89 272c 0d0a 2020   .........',..  
-00001a70: 2020 2020 2020 2020 2020 27e9 8089 e4b8            '.....
-00001a80: ade7 88b6 e789 a9e4 bbb6 3a20 2720 2b20  ..........: ' + 
-00001a90: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-00001aa0: 2020 2027 e697 a027 0d0a 2020 2020 2020     '...'..      
-00001ab0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00001ac0: 662e 6375 7272 656e 7420 6973 204e 6f6e  f.current is Non
-00001ad0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001ae0: 2020 2065 6c73 6520 6627 7b73 656c 662e     else f'{self.
-00001af0: 6375 7272 656e 742e 6974 656d 2e5f 5f63  current.item.__c
-00001b00: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
-00001b10: 2061 7420 7b69 6428 7365 6c66 2e63 7572   at {id(self.cur
-00001b20: 7265 6e74 2e69 7465 6d29 3a58 7d27 0d0a  rent.item):X}'..
-00001b30: 2020 2020 2020 2020 2020 2020 292c 0d0a              ),..
-00001b40: 2020 2020 2020 2020 2020 2020 27e9 8089              '...
-00001b50: e4b8 ade5 ad90 e789 a9e4 bbb6 3a20 2720  ............: ' 
-00001b60: 2b20 272c 2027 2e6a 6f69 6e28 0d0a 2020  + ', '.join(..  
-00001b70: 2020 2020 2020 2020 2020 2020 2020 280d                (.
-00001b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b90: 2020 2020 2066 275b 7b72 616e 6765 5b30       f'[{range[0
-00001ba0: 5d7d 5d27 0d0a 2020 2020 2020 2020 2020  ]}]'..          
-00001bb0: 2020 2020 2020 2020 2020 6966 2072 616e            if ran
-00001bc0: 6765 5b30 5d20 2b20 3120 3d3d 2072 616e  ge[0] + 1 == ran
-00001bd0: 6765 5b31 5d0d 0a20 2020 2020 2020 2020  ge[1]..         
-00001be0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00001bf0: 6627 5b7b 7261 6e67 655b 305d 7d3a 7b72  f'[{range[0]}:{r
-00001c00: 616e 6765 5b31 5d7d 5d27 0d0a 2020 2020  ange[1]}]'..    
-00001c10: 2020 2020 2020 2020 2020 2020 290d 0a20              ).. 
-00001c20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00001c30: 6f72 2072 616e 6765 2069 6e20 7261 6e67  or range in rang
-00001c40: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-00001c50: 290d 0a20 2020 2020 2020 205d 0d0a 0d0a  )..        ]....
-00001c60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00001c70: 6375 7272 656e 7420 6973 206e 6f74 204e  current is not N
-00001c80: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00001c90: 2020 702e 7365 7442 7275 7368 2851 436f    p.setBrush(QCo
-00001ca0: 6c6f 7228 3139 352c 2031 3331 2c20 3139  lor(195, 131, 19
-00001cb0: 2c20 3332 2929 0d0a 2020 2020 2020 2020  , 32))..        
-00001cc0: 2020 2020 702e 7365 7450 656e 2851 436f      p.setPen(QCo
-00001cd0: 6c6f 7228 3139 352c 2031 3331 2c20 3139  lor(195, 131, 19
-00001ce0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00001cf0: 702e 6472 6177 5265 6374 280d 0a20 2020  p.drawRect(..   
-00001d00: 2020 2020 2020 2020 2020 2020 2051 5265               QRe
-00001d10: 6374 4628 0d0a 2020 2020 2020 2020 2020  ctF(..          
-00001d20: 2020 2020 2020 2020 2020 5150 6f69 6e74            QPoint
-00001d30: 4628 7365 6c66 2e67 6c78 5f74 6f5f 6f76  F(self.glx_to_ov
-00001d40: 6572 6c61 795f 7828 7365 6c66 2e63 7572  erlay_x(self.cur
-00001d50: 7265 6e74 2e6d 696e 5f67 6c78 292c 2073  rent.min_glx), s
-00001d60: 656c 662e 676c 795f 746f 5f6f 7665 726c  elf.gly_to_overl
-00001d70: 6179 5f79 2873 656c 662e 6375 7272 656e  ay_y(self.curren
-00001d80: 742e 6d69 6e5f 676c 7929 292c 0d0a 2020  t.min_gly)),..  
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 5150 6f69 6e74 4628 7365 6c66 2e67    QPointF(self.g
-00001db0: 6c78 5f74 6f5f 6f76 6572 6c61 795f 7828  lx_to_overlay_x(
-00001dc0: 7365 6c66 2e63 7572 7265 6e74 2e6d 6178  self.current.max
-00001dd0: 5f67 6c78 292c 2073 656c 662e 676c 795f  _glx), self.gly_
-00001de0: 746f 5f6f 7665 726c 6179 5f79 2873 656c  to_overlay_y(sel
-00001df0: 662e 6375 7272 656e 742e 6d61 785f 676c  f.current.max_gl
-00001e00: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
-00001e10: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00001e20: 2020 2020 290d 0a0d 0a20 2020 2020 2020      )....       
-00001e30: 2020 2020 2070 2e73 6574 4272 7573 6828       p.setBrush(
-00001e40: 5143 6f6c 6f72 2831 3934 2c20 3130 322c  QColor(194, 102,
-00001e50: 2032 3139 2c20 3634 2929 0d0a 2020 2020   219, 64))..    
-00001e60: 2020 2020 2020 2020 702e 7365 7450 656e          p.setPen
-00001e70: 2851 436f 6c6f 7228 3139 342c 2031 3032  (QColor(194, 102
-00001e80: 2c20 3231 3929 290d 0a20 2020 2020 2020  , 219))..       
-00001e90: 2020 2020 2066 6f72 2063 6869 6c64 2069       for child i
-00001ea0: 6e20 7365 6c66 2e73 656c 6563 7465 645f  n self.selected_
-00001eb0: 6368 696c 6472 656e 3a0d 0a20 2020 2020  children:..     
-00001ec0: 2020 2020 2020 2020 2020 2070 2e64 7261             p.dra
-00001ed0: 7752 6563 7428 0d0a 2020 2020 2020 2020  wRect(..        
-00001ee0: 2020 2020 2020 2020 2020 2020 5152 6563              QRec
-00001ef0: 7446 280d 0a20 2020 2020 2020 2020 2020  tF(..           
-00001f00: 2020 2020 2020 2020 2020 2020 2051 506f               QPo
-00001f10: 696e 7446 2873 656c 662e 676c 785f 746f  intF(self.glx_to
-00001f20: 5f6f 7665 726c 6179 5f78 2863 6869 6c64  _overlay_x(child
-00001f30: 2e6d 696e 5f67 6c78 292c 2073 656c 662e  .min_glx), self.
-00001f40: 676c 795f 746f 5f6f 7665 726c 6179 5f79  gly_to_overlay_y
-00001f50: 2863 6869 6c64 2e6d 696e 5f67 6c79 2929  (child.min_gly))
-00001f60: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001f70: 2020 2020 2020 2020 2020 2051 506f 696e             QPoin
-00001f80: 7446 2873 656c 662e 676c 785f 746f 5f6f  tF(self.glx_to_o
-00001f90: 7665 726c 6179 5f78 2863 6869 6c64 2e6d  verlay_x(child.m
-00001fa0: 6178 5f67 6c78 292c 2073 656c 662e 676c  ax_glx), self.gl
-00001fb0: 795f 746f 5f6f 7665 726c 6179 5f79 2863  y_to_overlay_y(c
-00001fc0: 6869 6c64 2e6d 6178 5f67 6c79 2929 0d0a  hild.max_gly))..
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00001ff0: 2020 2020 2020 2029 0d0a 0d0a 2020 2020         )....    
-00002000: 2020 2020 702e 7365 7450 656e 2851 742e      p.setPen(Qt.
-00002010: 476c 6f62 616c 436f 6c6f 722e 7768 6974  GlobalColor.whit
-00002020: 6529 0d0a 2020 2020 2020 2020 702e 6472  e)..        p.dr
-00002030: 6177 5465 7874 2872 6563 742c 2051 742e  awText(rect, Qt.
-00002040: 416c 6967 6e6d 656e 7446 6c61 672e 416c  AlignmentFlag.Al
-00002050: 6967 6e4c 6566 7420 7c20 5174 2e41 6c69  ignLeft | Qt.Ali
-00002060: 676e 6d65 6e74 466c 6167 2e41 6c69 676e  gnmentFlag.Align
-00002070: 546f 702c 2027 5c6e 272e 6a6f 696e 2874  Top, '\n'.join(t
-00002080: 7874 5f6c 6973 7429 290d 0a              xt_list))..
+00000000: 0a66 726f 6d20 6461 7461 636c 6173 7365  .from dataclasse
+00000010: 7320 696d 706f 7274 2064 6174 6163 6c61  s import datacla
+00000020: 7373 0a66 726f 6d20 7479 7069 6e67 2069  ss.from typing i
+00000030: 6d70 6f72 7420 5459 5045 5f43 4845 434b  mport TYPE_CHECK
+00000040: 494e 470a 0a66 726f 6d20 5079 5369 6465  ING..from PySide
+00000050: 362e 5174 436f 7265 2069 6d70 6f72 7420  6.QtCore import 
+00000060: 5145 7665 6e74 2c20 514f 626a 6563 742c  QEvent, QObject,
+00000070: 2051 506f 696e 7446 2c20 5152 6563 7446   QPointF, QRectF
+00000080: 2c20 5174 0a66 726f 6d20 5079 5369 6465  , Qt.from PySide
+00000090: 362e 5174 4775 6920 696d 706f 7274 2051  6.QtGui import Q
+000000a0: 436f 6c6f 722c 2051 4d6f 7573 6545 7665  Color, QMouseEve
+000000b0: 6e74 2c20 5150 6169 6e74 6572 2c20 5150  nt, QPainter, QP
+000000c0: 6169 6e74 4576 656e 740a 0a66 726f 6d20  aintEvent..from 
+000000d0: 6a61 6e69 6d2e 616e 696d 732e 6469 7370  janim.anims.disp
+000000e0: 6c61 7920 696d 706f 7274 2044 6973 706c  lay import Displ
+000000f0: 6179 0a66 726f 6d20 6a61 6e69 6d2e 6974  ay.from janim.it
+00000100: 656d 732e 6974 656d 2069 6d70 6f72 7420  ems.item import 
+00000110: 4974 656d 0a66 726f 6d20 6a61 6e69 6d2e  Item.from janim.
+00000120: 6974 656d 732e 706f 696e 7473 2069 6d70  items.points imp
+00000130: 6f72 7420 506f 696e 7473 0a0a 6966 2054  ort Points..if T
+00000140: 5950 455f 4348 4543 4b49 4e47 3a0a 2020  YPE_CHECKING:.  
+00000150: 2020 6672 6f6d 206a 616e 696d 2e67 7569    from janim.gui
+00000160: 2e61 6e69 6d5f 7669 6577 6572 2069 6d70  .anim_viewer imp
+00000170: 6f72 7420 416e 696d 5669 6577 6572 0a0a  ort AnimViewer..
+00000180: 0a63 6c61 7373 2053 656c 6563 746f 7228  .class Selector(
+00000190: 514f 626a 6563 7429 3a0a 2020 2020 2727  QObject):.    ''
+000001a0: 270a 2020 2020 e5ad 90e7 89a9 e4bb b6e9  '.    ..........
+000001b0: 8089 e68b a9e5 b7a5 e585 b70a 2020 2020  ............    
+000001c0: 2727 270a 2020 2020 4064 6174 6163 6c61  '''.    @datacla
+000001d0: 7373 0a20 2020 2063 6c61 7373 2053 656c  ss.    class Sel
+000001e0: 6563 7465 6449 7465 6d3a 0a20 2020 2020  ectedItem:.     
+000001f0: 2020 2069 7465 6d3a 2049 7465 6d0a 2020     item: Item.  
+00000200: 2020 2020 2020 6d69 6e5f 676c 783a 2066        min_glx: f
+00000210: 6c6f 6174 0a20 2020 2020 2020 206d 696e  loat.        min
+00000220: 5f67 6c79 3a20 666c 6f61 740a 2020 2020  _gly: float.    
+00000230: 2020 2020 6d61 785f 676c 783a 2066 6c6f      max_glx: flo
+00000240: 6174 0a20 2020 2020 2020 206d 6178 5f67  at.        max_g
+00000250: 6c79 3a20 666c 6f61 740a 0a20 2020 2064  ly: float..    d
+00000260: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00000270: 2c20 7061 7265 6e74 3a20 2741 6e69 6d56  , parent: 'AnimV
+00000280: 6965 7765 7227 2920 2d3e 204e 6f6e 653a  iewer') -> None:
+00000290: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+000002a0: 2e5f 5f69 6e69 745f 5f28 7061 7265 6e74  .__init__(parent
+000002b0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+000002c0: 6965 7765 7220 3d20 7061 7265 6e74 0a0a  iewer = parent..
+000002d0: 2020 2020 2020 2020 7365 6c66 2e76 6965          self.vie
+000002e0: 7765 722e 676c 772e 696e 7374 616c 6c45  wer.glw.installE
+000002f0: 7665 6e74 4669 6c74 6572 2873 656c 6629  ventFilter(self)
+00000300: 0a20 2020 2020 2020 2073 656c 662e 7669  .        self.vi
+00000310: 6577 6572 2e6f 7665 726c 6179 2e69 6e73  ewer.overlay.ins
+00000320: 7461 6c6c 4576 656e 7446 696c 7465 7228  tallEventFilter(
+00000330: 7365 6c66 290a 0a20 2020 2020 2020 2073  self)..        s
+00000340: 656c 662e 636c 6561 7228 290a 0a20 2020  elf.clear()..   
+00000350: 2064 6566 2063 6c65 6172 2873 656c 6629   def clear(self)
+00000360: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00000370: 2020 7365 6c66 2e63 7572 7265 6e74 3a20    self.current: 
+00000380: 5365 6c65 6374 6f72 2e53 656c 6563 7465  Selector.Selecte
+00000390: 6449 7465 6d20 7c20 4e6f 6e65 203d 204e  dItem | None = N
+000003a0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+000003b0: 2e63 6869 6c64 7265 6e3a 206c 6973 745b  .children: list[
+000003c0: 5365 6c65 6374 6f72 2e53 656c 6563 7465  Selector.Selecte
+000003d0: 6449 7465 6d5d 203d 205b 5d0a 2020 2020  dItem] = [].    
+000003e0: 2020 2020 7365 6c66 2e73 656c 6563 7465      self.selecte
+000003f0: 645f 6368 696c 6472 656e 3a20 6c69 7374  d_children: list
+00000400: 5b53 656c 6563 746f 722e 5365 6c65 6374  [Selector.Select
+00000410: 6564 4974 656d 5d20 3d20 5b5d 0a20 2020  edItem] = [].   
+00000420: 2020 2020 2073 656c 662e 7669 6577 6572       self.viewer
+00000430: 2e6f 7665 726c 6179 2e75 7064 6174 6528  .overlay.update(
+00000440: 290a 0a20 2020 2064 6566 2067 6c78 5f74  )..    def glx_t
+00000450: 6f5f 6f76 6572 6c61 795f 7828 7365 6c66  o_overlay_x(self
+00000460: 2c20 676c 783a 2066 6c6f 6174 2920 2d3e  , glx: float) ->
+00000470: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
+00000480: 7265 7475 726e 2028 676c 7820 2b20 3129  return (glx + 1)
+00000490: 202f 2032 202a 2073 656c 662e 7669 6577   / 2 * self.view
+000004a0: 6572 2e6f 7665 726c 6179 2e77 6964 7468  er.overlay.width
+000004b0: 2829 0a0a 2020 2020 6465 6620 676c 795f  ()..    def gly_
+000004c0: 746f 5f6f 7665 726c 6179 5f79 2873 656c  to_overlay_y(sel
+000004d0: 662c 2067 6c79 3a20 666c 6f61 7429 202d  f, gly: float) -
+000004e0: 3e20 666c 6f61 743a 0a20 2020 2020 2020  > float:.       
+000004f0: 2072 6574 7572 6e20 282d 676c 7920 2b20   return (-gly + 
+00000500: 3129 202f 2032 202a 2073 656c 662e 7669  1) / 2 * self.vi
+00000510: 6577 6572 2e6f 7665 726c 6179 2e68 6569  ewer.overlay.hei
+00000520: 6768 7428 290a 0a20 2020 2064 6566 2065  ght()..    def e
+00000530: 7665 6e74 4669 6c74 6572 2873 656c 662c  ventFilter(self,
+00000540: 2077 6174 6368 6564 3a20 514f 626a 6563   watched: QObjec
+00000550: 742c 2065 7665 6e74 3a20 5145 7665 6e74  t, event: QEvent
+00000560: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00000570: 2020 2069 6620 7761 7463 6865 6420 6973     if watched is
+00000580: 2073 656c 662e 7669 6577 6572 2e67 6c77   self.viewer.glw
+00000590: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000005a0: 2065 7665 6e74 2e74 7970 6528 2920 696e   event.type() in
+000005b0: 2028 5145 7665 6e74 2e54 7970 652e 4d6f   (QEvent.Type.Mo
+000005c0: 7573 6542 7574 746f 6e50 7265 7373 2c20  useButtonPress, 
+000005d0: 5145 7665 6e74 2e54 7970 652e 4d6f 7573  QEvent.Type.Mous
+000005e0: 6542 7574 746f 6e44 626c 436c 6963 6b29  eButtonDblClick)
+000005f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000600: 2020 7365 6c66 2e6f 6e5f 676c 775f 6d6f    self.on_glw_mo
+00000610: 7573 655f 7072 6573 7328 6576 656e 7429  use_press(event)
+00000620: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00000630: 6576 656e 742e 7479 7065 2829 203d 3d20  event.type() == 
+00000640: 5145 7665 6e74 2e54 7970 652e 4d6f 7573  QEvent.Type.Mous
+00000650: 654d 6f76 653a 0a20 2020 2020 2020 2020  eMove:.         
+00000660: 2020 2020 2020 2073 656c 662e 6f6e 5f67         self.on_g
+00000670: 6c77 5f6d 6f75 7365 5f6d 6f76 6528 6576  lw_mouse_move(ev
+00000680: 656e 7429 0a0a 2020 2020 2020 2020 6966  ent)..        if
+00000690: 2077 6174 6368 6564 2069 7320 7365 6c66   watched is self
+000006a0: 2e76 6965 7765 722e 6f76 6572 6c61 793a  .viewer.overlay:
+000006b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000006c0: 6576 656e 742e 7479 7065 2829 203d 3d20  event.type() == 
+000006d0: 5145 7665 6e74 2e54 7970 652e 5061 696e  QEvent.Type.Pain
+000006e0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+000006f0: 2020 2073 656c 662e 6f6e 5f6f 7665 726c     self.on_overl
+00000700: 6179 5f70 6169 6e74 2865 7665 6e74 290a  ay_paint(event).
+00000710: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000720: 7375 7065 7228 292e 6576 656e 7446 696c  super().eventFil
+00000730: 7465 7228 7761 7463 6865 642c 2065 7665  ter(watched, eve
+00000740: 6e74 290a 0a20 2020 2064 6566 206f 6e5f  nt)..    def on_
+00000750: 676c 775f 6d6f 7573 655f 7072 6573 7328  glw_mouse_press(
+00000760: 7365 6c66 2c20 6576 656e 743a 2051 4d6f  self, event: QMo
+00000770: 7573 6545 7665 6e74 2920 2d3e 204e 6f6e  useEvent) -> Non
+00000780: 653a 0a20 2020 2020 2020 2069 6620 6576  e:.        if ev
+00000790: 656e 742e 6d6f 6469 6669 6572 7328 2920  ent.modifiers() 
+000007a0: 2620 5174 2e4b 6579 626f 6172 644d 6f64  & Qt.KeyboardMod
+000007b0: 6966 6965 722e 436f 6e74 726f 6c4d 6f64  ifier.ControlMod
+000007c0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+000007d0: 2020 206d 6174 6368 2065 7665 6e74 2e62     match event.b
+000007e0: 7574 746f 6e28 293a 0a20 2020 2020 2020  utton():.       
+000007f0: 2020 2020 2020 2020 2063 6173 6520 5174           case Qt
+00000800: 2e4d 6f75 7365 4275 7474 6f6e 2e4c 6566  .MouseButton.Lef
+00000810: 7442 7574 746f 6e3a 0a20 2020 2020 2020  tButton:.       
+00000820: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000830: 662e 7365 6c65 6374 5f70 6172 656e 745f  f.select_parent_
+00000840: 6974 656d 2865 7665 6e74 290a 2020 2020  item(event).    
+00000850: 2020 2020 2020 2020 2020 2020 6361 7365              case
+00000860: 2051 742e 4d6f 7573 6542 7574 746f 6e2e   Qt.MouseButton.
+00000870: 5269 6768 7442 7574 746f 6e3a 0a20 2020  RightButton:.   
+00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000890: 2073 656c 662e 6465 6c65 7465 4c61 7465   self.deleteLate
+000008a0: 7228 290a 2020 2020 2020 2020 656c 7365  r().        else
+000008b0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+000008c0: 7463 6820 6576 656e 742e 6275 7474 6f6e  tch event.button
+000008d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000008e0: 2020 2020 6361 7365 2051 742e 4d6f 7573      case Qt.Mous
+000008f0: 6542 7574 746f 6e2e 4c65 6674 4275 7474  eButton.LeftButt
+00000900: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00000910: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
+00000920: 6563 745f 6368 696c 645f 6974 656d 2865  ect_child_item(e
+00000930: 7665 6e74 290a 2020 2020 2020 2020 2020  vent).          
+00000940: 2020 2020 2020 6361 7365 2051 742e 4d6f        case Qt.Mo
+00000950: 7573 6542 7574 746f 6e2e 5269 6768 7442  useButton.RightB
+00000960: 7574 746f 6e3a 0a20 2020 2020 2020 2020  utton:.         
+00000970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000980: 7265 6d6f 7665 5f63 6869 6c64 5f69 7465  remove_child_ite
+00000990: 6d28 6576 656e 7429 0a0a 2020 2020 2020  m(event)..      
+000009a0: 2020 7365 6c66 2e76 6965 7765 722e 6f76    self.viewer.ov
+000009b0: 6572 6c61 792e 7570 6461 7465 2829 0a0a  erlay.update()..
+000009c0: 2020 2020 6465 6620 6f6e 5f67 6c77 5f6d      def on_glw_m
+000009d0: 6f75 7365 5f6d 6f76 6528 7365 6c66 2c20  ouse_move(self, 
+000009e0: 6576 656e 743a 2051 4d6f 7573 6545 7665  event: QMouseEve
+000009f0: 6e74 2920 2d3e 204e 6f6e 653a 0a20 2020  nt) -> None:.   
+00000a00: 2020 2020 2069 6620 6e6f 7420 6576 656e       if not even
+00000a10: 742e 6d6f 6469 6669 6572 7328 2920 2620  t.modifiers() & 
+00000a20: 5174 2e4b 6579 626f 6172 644d 6f64 6966  Qt.KeyboardModif
+00000a30: 6965 722e 436f 6e74 726f 6c4d 6f64 6966  ier.ControlModif
+00000a40: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
+00000a50: 206d 6174 6368 2065 7665 6e74 2e62 7574   match event.but
+00000a60: 746f 6e73 2829 3a0a 2020 2020 2020 2020  tons():.        
+00000a70: 2020 2020 2020 2020 6361 7365 2051 742e          case Qt.
+00000a80: 4d6f 7573 6542 7574 746f 6e2e 4c65 6674  MouseButton.Left
+00000a90: 4275 7474 6f6e 3a0a 2020 2020 2020 2020  Button:.        
+00000aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00000ab0: 2e73 656c 6563 745f 6368 696c 645f 6974  .select_child_it
+00000ac0: 656d 2865 7665 6e74 290a 2020 2020 2020  em(event).      
+00000ad0: 2020 2020 2020 2020 2020 6361 7365 2051            case Q
+00000ae0: 742e 4d6f 7573 6542 7574 746f 6e2e 5269  t.MouseButton.Ri
+00000af0: 6768 7442 7574 746f 6e3a 0a20 2020 2020  ghtButton:.     
+00000b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000b10: 656c 662e 7265 6d6f 7665 5f63 6869 6c64  elf.remove_child
+00000b20: 5f69 7465 6d28 6576 656e 7429 0a0a 2020  _item(event)..  
+00000b30: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+00000b40: 6965 7765 722e 6f76 6572 6c61 792e 7570  iewer.overlay.up
+00000b50: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+00000b60: 7365 6c65 6374 5f70 6172 656e 745f 6974  select_parent_it
+00000b70: 656d 2873 656c 662c 2065 7665 6e74 3a20  em(self, event: 
+00000b80: 514d 6f75 7365 4576 656e 7429 202d 3e20  QMouseEvent) -> 
+00000b90: 4e6f 6e65 3a0a 2020 2020 2020 2020 7365  None:.        se
+00000ba0: 6c66 2e63 6869 6c64 7265 6e2e 636c 6561  lf.children.clea
+00000bb0: 7228 290a 2020 2020 2020 2020 7365 6c66  r().        self
+00000bc0: 2e73 656c 6563 7465 645f 6368 696c 6472  .selected_childr
+00000bd0: 656e 2e63 6c65 6172 2829 0a0a 2020 2020  en.clear()..    
+00000be0: 2020 2020 782c 2079 203d 2065 7665 6e74      x, y = event
+00000bf0: 2e70 6f73 6974 696f 6e28 292e 746f 5475  .position().toTu
+00000c00: 706c 6528 290a 2020 2020 2020 2020 676c  ple().        gl
+00000c10: 7820 3d20 7820 2f20 7365 6c66 2e76 6965  x = x / self.vie
+00000c20: 7765 722e 676c 772e 7769 6474 6828 2920  wer.glw.width() 
+00000c30: 2a20 3220 2d20 310a 2020 2020 2020 2020  * 2 - 1.        
+00000c40: 676c 7920 3d20 7920 2f20 7365 6c66 2e76  gly = y / self.v
+00000c50: 6965 7765 722e 676c 772e 6865 6967 6874  iewer.glw.height
+00000c60: 2829 202a 202d 3220 2b20 310a 0a20 2020  () * -2 + 1..   
+00000c70: 2020 2020 2061 6e69 6d20 3d20 7365 6c66       anim = self
+00000c80: 2e76 6965 7765 722e 616e 696d 0a20 2020  .viewer.anim.   
+00000c90: 2020 2020 2067 6c6f 6261 6c5f 7420 3d20       global_t = 
+00000ca0: 616e 696d 2e5f 7469 6d65 0a20 2020 2020  anim._time.     
+00000cb0: 2020 2063 616d 6572 615f 696e 666f 203d     camera_info =
+00000cc0: 2061 6e69 6d2e 7469 6d65 6c69 6e65 2e63   anim.timeline.c
+00000cd0: 616d 6572 612e 6375 7272 656e 7428 6173  amera.current(as
+00000ce0: 5f74 696d 653d 676c 6f62 616c 5f74 292e  _time=global_t).
+00000cf0: 706f 696e 7473 2e69 6e66 6f0a 0a20 2020  points.info..   
+00000d00: 2020 2020 2066 6f75 6e64 3a20 6c69 7374       found: list
+00000d10: 5b53 656c 6563 746f 722e 5365 6c65 6374  [Selector.Select
+00000d20: 6564 4974 656d 5d20 3d20 5b5d 0a0a 2020  edItem] = []..  
+00000d30: 2020 2020 2020 666f 7220 6469 7370 6c61        for displa
+00000d40: 7920 696e 2061 6e69 6d2e 6469 7370 6c61  y in anim.displa
+00000d50: 795f 616e 696d 2e61 6e69 6d73 3a0a 2020  y_anim.anims:.  
+00000d60: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+00000d70: 793a 2044 6973 706c 6179 0a20 2020 2020  y: Display.     
+00000d80: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
+00000d90: 7370 6c61 792e 676c 6f62 616c 5f72 616e  splay.global_ran
+00000da0: 6765 2e61 7420 3c3d 2067 6c6f 6261 6c5f  ge.at <= global_
+00000db0: 7420 3c20 6469 7370 6c61 792e 676c 6f62  t < display.glob
+00000dc0: 616c 5f72 616e 6765 2e65 6e64 3a0a 2020  al_range.end:.  
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000de0: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+00000df0: 2020 2020 626f 7820 3d20 6469 7370 6c61      box = displa
+00000e00: 792e 6974 656d 2e63 7572 7265 6e74 2861  y.item.current(a
+00000e10: 735f 7469 6d65 3d67 6c6f 6261 6c5f 7429  s_time=global_t)
+00000e20: 2850 6f69 6e74 7329 2e70 6f69 6e74 732e  (Points).points.
+00000e30: 626f 780a 0a20 2020 2020 2020 2020 2020  box..           
+00000e40: 206d 6170 7065 6420 3d20 6361 6d65 7261   mapped = camera
+00000e50: 5f69 6e66 6f2e 6d61 705f 706f 696e 7473  _info.map_points
+00000e60: 2862 6f78 2e67 6574 5f63 6f72 6e65 7273  (box.get_corners
+00000e70: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00000e80: 6d69 6e5f 676c 782c 206d 696e 5f67 6c79  min_glx, min_gly
+00000e90: 203d 206d 6170 7065 642e 6d69 6e28 6178   = mapped.min(ax
+00000ea0: 6973 3d30 290a 2020 2020 2020 2020 2020  is=0).          
+00000eb0: 2020 6d61 785f 676c 782c 206d 6178 5f67    max_glx, max_g
+00000ec0: 6c79 203d 206d 6170 7065 642e 6d61 7828  ly = mapped.max(
+00000ed0: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+00000ee0: 2020 2020 6966 206e 6f74 206d 696e 5f67      if not min_g
+00000ef0: 6c78 203c 3d20 676c 7820 3c3d 206d 6178  lx <= glx <= max
+00000f00: 5f67 6c78 206f 7220 6e6f 7420 6d69 6e5f  _glx or not min_
+00000f10: 676c 7920 3c3d 2067 6c79 203c 3d20 6d61  gly <= gly <= ma
+00000f20: 785f 676c 793a 0a20 2020 2020 2020 2020  x_gly:.         
+00000f30: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00000f40: 0a20 2020 2020 2020 2020 2020 2066 6f75  .            fou
+00000f50: 6e64 2e61 7070 656e 6428 5365 6c65 6374  nd.append(Select
+00000f60: 6f72 2e53 656c 6563 7465 6449 7465 6d28  or.SelectedItem(
+00000f70: 6469 7370 6c61 792e 6974 656d 2c20 6d69  display.item, mi
+00000f80: 6e5f 676c 782c 206d 696e 5f67 6c79 2c20  n_glx, min_gly, 
+00000f90: 6d61 785f 676c 782c 206d 6178 5f67 6c79  max_glx, max_gly
+00000fa0: 2929 0a0a 2020 2020 2020 2020 6966 206e  ))..        if n
+00000fb0: 6f74 2066 6f75 6e64 3a0a 2020 2020 2020  ot found:.      
+00000fc0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+00000fd0: 6e74 203d 204e 6f6e 650a 2020 2020 2020  nt = None.      
+00000fe0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00000ff0: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
+00001000: 656e 7420 6973 204e 6f6e 6520 6f72 2073  ent is None or s
+00001010: 656c 662e 6375 7272 656e 7420 6e6f 7420  elf.current not 
+00001020: 696e 2066 6f75 6e64 3a0a 2020 2020 2020  in found:.      
+00001030: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00001040: 7572 7265 6e74 203d 2066 6f75 6e64 5b30  urrent = found[0
+00001050: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00001060: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00001070: 2020 2020 6964 7820 3d20 666f 756e 642e      idx = found.
+00001080: 696e 6465 7828 7365 6c66 2e63 7572 7265  index(self.curre
+00001090: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+000010a0: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
+000010b0: 203d 2066 6f75 6e64 5b28 6964 7820 2b20   = found[(idx + 
+000010c0: 3129 2025 206c 656e 2866 6f75 6e64 295d  1) % len(found)]
+000010d0: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+000010e0: 7220 6974 656d 2069 6e20 7365 6c66 2e63  r item in self.c
+000010f0: 7572 7265 6e74 2e69 7465 6d2e 6765 745f  urrent.item.get_
+00001100: 6368 696c 6472 656e 2829 3a0a 2020 2020  children():.    
+00001110: 2020 2020 2020 2020 2020 2020 626f 7820              box 
+00001120: 3d20 6974 656d 2e63 7572 7265 6e74 2861  = item.current(a
+00001130: 735f 7469 6d65 3d67 6c6f 6261 6c5f 7429  s_time=global_t)
+00001140: 2850 6f69 6e74 7329 2e70 6f69 6e74 732e  (Points).points.
+00001150: 626f 780a 2020 2020 2020 2020 2020 2020  box.            
+00001160: 2020 2020 6d61 7070 6564 203d 2063 616d      mapped = cam
+00001170: 6572 615f 696e 666f 2e6d 6170 5f70 6f69  era_info.map_poi
+00001180: 6e74 7328 626f 782e 6765 745f 636f 726e  nts(box.get_corn
+00001190: 6572 7328 2929 0a20 2020 2020 2020 2020  ers()).         
+000011a0: 2020 2020 2020 2073 656c 662e 6368 696c         self.chil
+000011b0: 6472 656e 2e61 7070 656e 6428 5365 6c65  dren.append(Sele
+000011c0: 6374 6f72 2e53 656c 6563 7465 6449 7465  ctor.SelectedIte
+000011d0: 6d28 6974 656d 2c20 2a6d 6170 7065 642e  m(item, *mapped.
+000011e0: 6d69 6e28 6178 6973 3d30 292c 202a 6d61  min(axis=0), *ma
+000011f0: 7070 6564 2e6d 6178 2861 7869 733d 3029  pped.max(axis=0)
+00001200: 2929 0a0a 2020 2020 6465 6620 7365 6c65  ))..    def sele
+00001210: 6374 5f63 6869 6c64 5f69 7465 6d28 7365  ct_child_item(se
+00001220: 6c66 2c20 6576 656e 743a 2051 4d6f 7573  lf, event: QMous
+00001230: 6545 7665 6e74 2920 2d3e 204e 6f6e 653a  eEvent) -> None:
+00001240: 0a20 2020 2020 2020 2078 2c20 7920 3d20  .        x, y = 
+00001250: 6576 656e 742e 706f 7369 7469 6f6e 2829  event.position()
+00001260: 2e74 6f54 7570 6c65 2829 0a20 2020 2020  .toTuple().     
+00001270: 2020 2067 6c78 203d 2078 202f 2073 656c     glx = x / sel
+00001280: 662e 7669 6577 6572 2e67 6c77 2e77 6964  f.viewer.glw.wid
+00001290: 7468 2829 202a 2032 202d 2031 0a20 2020  th() * 2 - 1.   
+000012a0: 2020 2020 2067 6c79 203d 2079 202f 2073       gly = y / s
+000012b0: 656c 662e 7669 6577 6572 2e67 6c77 2e68  elf.viewer.glw.h
+000012c0: 6569 6768 7428 2920 2a20 2d32 202b 2031  eight() * -2 + 1
+000012d0: 0a0a 2020 2020 2020 2020 666f 7220 6368  ..        for ch
+000012e0: 696c 6420 696e 2073 656c 662e 6368 696c  ild in self.chil
+000012f0: 6472 656e 3a0a 2020 2020 2020 2020 2020  dren:.          
+00001300: 2020 6966 2063 6869 6c64 2069 6e20 7365    if child in se
+00001310: 6c66 2e73 656c 6563 7465 645f 6368 696c  lf.selected_chil
+00001320: 6472 656e 3a0a 2020 2020 2020 2020 2020  dren:.          
+00001330: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00001340: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00001350: 7420 6368 696c 642e 6d69 6e5f 676c 7820  t child.min_glx 
+00001360: 3c3d 2067 6c78 203c 3d20 6368 696c 642e  <= glx <= child.
+00001370: 6d61 785f 676c 7820 6f72 206e 6f74 2063  max_glx or not c
+00001380: 6869 6c64 2e6d 696e 5f67 6c79 203c 3d20  hild.min_gly <= 
+00001390: 676c 7920 3c3d 2063 6869 6c64 2e6d 6178  gly <= child.max
+000013a0: 5f67 6c79 3a0a 2020 2020 2020 2020 2020  _gly:.          
+000013b0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+000013c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000013d0: 7365 6c65 6374 6564 5f63 6869 6c64 7265  selected_childre
+000013e0: 6e2e 6170 7065 6e64 2863 6869 6c64 290a  n.append(child).
+000013f0: 0a20 2020 2064 6566 2072 656d 6f76 655f  .    def remove_
+00001400: 6368 696c 645f 6974 656d 2873 656c 662c  child_item(self,
+00001410: 2065 7665 6e74 3a20 514d 6f75 7365 4576   event: QMouseEv
+00001420: 656e 7429 202d 3e20 4e6f 6e65 3a0a 2020  ent) -> None:.  
+00001430: 2020 2020 2020 782c 2079 203d 2065 7665        x, y = eve
+00001440: 6e74 2e70 6f73 6974 696f 6e28 292e 746f  nt.position().to
+00001450: 5475 706c 6528 290a 2020 2020 2020 2020  Tuple().        
+00001460: 676c 7820 3d20 7820 2f20 7365 6c66 2e76  glx = x / self.v
+00001470: 6965 7765 722e 676c 772e 7769 6474 6828  iewer.glw.width(
+00001480: 2920 2a20 3220 2d20 310a 2020 2020 2020  ) * 2 - 1.      
+00001490: 2020 676c 7920 3d20 7920 2f20 7365 6c66    gly = y / self
+000014a0: 2e76 6965 7765 722e 676c 772e 6865 6967  .viewer.glw.heig
+000014b0: 6874 2829 202a 202d 3220 2b20 310a 0a20  ht() * -2 + 1.. 
+000014c0: 2020 2020 2020 2066 6f72 2063 6869 6c64         for child
+000014d0: 2069 6e20 7365 6c66 2e73 656c 6563 7465   in self.selecte
+000014e0: 645f 6368 696c 6472 656e 3a0a 2020 2020  d_children:.    
+000014f0: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00001500: 6869 6c64 2e6d 696e 5f67 6c78 203c 3d20  hild.min_glx <= 
+00001510: 676c 7820 3c3d 2063 6869 6c64 2e6d 6178  glx <= child.max
+00001520: 5f67 6c78 206f 7220 6e6f 7420 6368 696c  _glx or not chil
+00001530: 642e 6d69 6e5f 676c 7920 3c3d 2067 6c79  d.min_gly <= gly
+00001540: 203c 3d20 6368 696c 642e 6d61 785f 676c   <= child.max_gl
+00001550: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00001560: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00001570: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
+00001580: 6563 7465 645f 6368 696c 6472 656e 2e72  ected_children.r
+00001590: 656d 6f76 6528 6368 696c 6429 0a0a 2020  emove(child)..  
+000015a0: 2020 6465 6620 6f6e 5f6f 7665 726c 6179    def on_overlay
+000015b0: 5f70 6169 6e74 2873 656c 662c 2065 7665  _paint(self, eve
+000015c0: 6e74 3a20 5150 6169 6e74 4576 656e 7429  nt: QPaintEvent)
+000015d0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+000015e0: 2020 7265 6374 203d 2073 656c 662e 7669    rect = self.vi
+000015f0: 6577 6572 2e6f 7665 726c 6179 2e72 6563  ewer.overlay.rec
+00001600: 7428 292e 6164 6a75 7374 6564 2832 2c20  t().adjusted(2, 
+00001610: 322c 202d 322c 202d 3229 0a0a 2020 2020  2, -2, -2)..    
+00001620: 2020 2020 7020 3d20 5150 6169 6e74 6572      p = QPainter
+00001630: 2873 656c 662e 7669 6577 6572 2e6f 7665  (self.viewer.ove
+00001640: 726c 6179 290a 0a20 2020 2020 2020 2072  rlay)..        r
+00001650: 616e 6765 733a 206c 6973 745b 7475 706c  anges: list[tupl
+00001660: 655b 666c 6f61 742c 2066 6c6f 6174 5d5d  e[float, float]]
+00001670: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+00001680: 2073 656c 662e 7365 6c65 6374 6564 5f63   self.selected_c
+00001690: 6869 6c64 7265 6e3a 0a20 2020 2020 2020  hildren:.       
+000016a0: 2020 2020 2072 616e 6765 5f73 7461 7274       range_start
+000016b0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000016c0: 2020 2020 7261 6e67 655f 656e 6420 3d20      range_end = 
+000016d0: 4e6f 6e65 0a0a 2020 2020 2020 2020 2020  None..          
+000016e0: 2020 666f 7220 692c 2063 6869 6c64 2069    for i, child i
+000016f0: 6e20 656e 756d 6572 6174 6528 7365 6c66  n enumerate(self
+00001700: 2e63 6869 6c64 7265 6e29 3a0a 2020 2020  .children):.    
+00001710: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00001720: 6869 6c64 2069 6e20 7365 6c66 2e73 656c  hild in self.sel
+00001730: 6563 7465 645f 6368 696c 6472 656e 3a0a  ected_children:.
+00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001750: 2020 2020 6966 2072 616e 6765 5f73 7461      if range_sta
+00001760: 7274 2069 7320 4e6f 6e65 3a0a 2020 2020  rt is None:.    
+00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001780: 2020 2020 7261 6e67 655f 7374 6172 7420      range_start 
+00001790: 3d20 690a 2020 2020 2020 2020 2020 2020  = i.            
+000017a0: 2020 2020 2020 2020 2020 2020 7261 6e67              rang
+000017b0: 655f 656e 6420 3d20 6920 2b20 310a 2020  e_end = i + 1.  
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2020 2020 6966 2069 203d 3d20 7261 6e67      if i == rang
+00001800: 655f 656e 643a 0a20 2020 2020 2020 2020  e_end:.         
+00001810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001820: 616e 6765 5f65 6e64 202b 3d20 310a 2020  ange_end += 1.  
+00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001840: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 7261 6e67 6573 2e61 7070 656e 6428 2872  ranges.append((r
+00001870: 616e 6765 5f73 7461 7274 2c20 7261 6e67  ange_start, rang
+00001880: 655f 656e 6429 290a 2020 2020 2020 2020  e_end)).        
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 7261 6e67 655f 7374 6172 7420 3d20 690a  range_start = i.
+000018b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018c0: 2020 2020 2020 2020 7261 6e67 655f 656e          range_en
+000018d0: 6420 3d20 6920 2b20 310a 2020 2020 2020  d = i + 1.      
+000018e0: 2020 2020 2020 7261 6e67 6573 2e61 7070        ranges.app
+000018f0: 656e 6428 2872 616e 6765 5f73 7461 7274  end((range_start
+00001900: 2c20 7261 6e67 655f 656e 6429 290a 0a20  , range_end)).. 
+00001910: 2020 2020 2020 2074 7874 5f6c 6973 7420         txt_list 
+00001920: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00001930: 27e5 ad90 e789 a9e4 bbb6 e980 89e6 8ba9  '...............
+00001940: e5b7 a5e5 85b7 efbc 8843 7472 6c2b e5b7  .........Ctrl+..
+00001950: a6e9 94ae 3a20 e980 89e6 8ba9 e788 b6e7  ....: ..........
+00001960: 89a9 e4bb b6ef bc8c e5b7 a6e9 94ae 3a20  ..............: 
+00001970: e980 89e6 8ba9 e5ad 90e7 89a9 e4bb b6ef  ................
+00001980: bc8c e58f b3e9 94ae 3a20 e58f 96e6 b688  ........: ......
+00001990: e980 89e6 8ba9 e5ad 90e7 89a9 e4bb b6ef  ................
+000019a0: bc8c 4374 726c 2be5 8fb3 e994 ae3a 20e9  ..Ctrl+......: .
+000019b0: 8080 e587 baef bc89 272c 0a20 2020 2020  ........',.     
+000019c0: 2020 2020 2020 2027 e980 89e4 b8ad e788         '........
+000019d0: b6e7 89a9 e4bb b63a 2027 202b 2028 0a20  .......: ' + (. 
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000019f0: e697 a027 0a20 2020 2020 2020 2020 2020  ...'.           
+00001a00: 2020 2020 2069 6620 7365 6c66 2e63 7572       if self.cur
+00001a10: 7265 6e74 2069 7320 4e6f 6e65 0a20 2020  rent is None.   
+00001a20: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00001a30: 6520 6627 7b73 656c 662e 6375 7272 656e  e f'{self.curren
+00001a40: 742e 6974 656d 2e5f 5f63 6c61 7373 5f5f  t.item.__class__
+00001a50: 2e5f 5f6e 616d 655f 5f7d 2061 7420 7b69  .__name__} at {i
+00001a60: 6428 7365 6c66 2e63 7572 7265 6e74 2e69  d(self.current.i
+00001a70: 7465 6d29 3a58 7d27 0a20 2020 2020 2020  tem):X}'.       
+00001a80: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00001a90: 2020 2020 27e9 8089 e4b8 ade5 ad90 e789      '...........
+00001aa0: a9e4 bbb6 3a20 2720 2b20 272c 2027 2e6a  ....: ' + ', '.j
+00001ab0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+00001ac0: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
+00001ad0: 2020 2020 2020 2020 2020 2066 275b 7b72             f'[{r
+00001ae0: 616e 6765 5b30 5d7d 5d27 0a20 2020 2020  ange[0]}]'.     
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001b00: 6620 7261 6e67 655b 305d 202b 2031 203d  f range[0] + 1 =
+00001b10: 3d20 7261 6e67 655b 315d 0a20 2020 2020  = range[1].     
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00001b30: 6c73 6520 6627 5b7b 7261 6e67 655b 305d  lse f'[{range[0]
+00001b40: 7d3a 7b72 616e 6765 5b31 5d7d 5d27 0a20  }:{range[1]}]'. 
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b70: 2066 6f72 2072 616e 6765 2069 6e20 7261   for range in ra
+00001b80: 6e67 6573 0a20 2020 2020 2020 2020 2020  nges.           
+00001b90: 2029 0a20 2020 2020 2020 205d 0a0a 2020   ).        ]..  
+00001ba0: 2020 2020 2020 6966 2073 656c 662e 6375        if self.cu
+00001bb0: 7272 656e 7420 6973 206e 6f74 204e 6f6e  rrent is not Non
+00001bc0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00001bd0: 2e73 6574 4272 7573 6828 5143 6f6c 6f72  .setBrush(QColor
+00001be0: 2831 3935 2c20 3133 312c 2031 392c 2033  (195, 131, 19, 3
+00001bf0: 3229 290a 2020 2020 2020 2020 2020 2020  2)).            
+00001c00: 702e 7365 7450 656e 2851 436f 6c6f 7228  p.setPen(QColor(
+00001c10: 3139 352c 2031 3331 2c20 3139 2929 0a20  195, 131, 19)). 
+00001c20: 2020 2020 2020 2020 2020 2070 2e64 7261             p.dra
+00001c30: 7752 6563 7428 0a20 2020 2020 2020 2020  wRect(.         
+00001c40: 2020 2020 2020 2051 5265 6374 4628 0a20         QRectF(. 
+00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c60: 2020 2051 506f 696e 7446 2873 656c 662e     QPointF(self.
+00001c70: 676c 785f 746f 5f6f 7665 726c 6179 5f78  glx_to_overlay_x
+00001c80: 2873 656c 662e 6375 7272 656e 742e 6d69  (self.current.mi
+00001c90: 6e5f 676c 7829 2c20 7365 6c66 2e67 6c79  n_glx), self.gly
+00001ca0: 5f74 6f5f 6f76 6572 6c61 795f 7928 7365  _to_overlay_y(se
+00001cb0: 6c66 2e63 7572 7265 6e74 2e6d 696e 5f67  lf.current.min_g
+00001cc0: 6c79 2929 2c0a 2020 2020 2020 2020 2020  ly)),.          
+00001cd0: 2020 2020 2020 2020 2020 5150 6f69 6e74            QPoint
+00001ce0: 4628 7365 6c66 2e67 6c78 5f74 6f5f 6f76  F(self.glx_to_ov
+00001cf0: 6572 6c61 795f 7828 7365 6c66 2e63 7572  erlay_x(self.cur
+00001d00: 7265 6e74 2e6d 6178 5f67 6c78 292c 2073  rent.max_glx), s
+00001d10: 656c 662e 676c 795f 746f 5f6f 7665 726c  elf.gly_to_overl
+00001d20: 6179 5f79 2873 656c 662e 6375 7272 656e  ay_y(self.curren
+00001d30: 742e 6d61 785f 676c 7929 290a 2020 2020  t.max_gly)).    
+00001d40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001d50: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00001d60: 2020 2020 2020 2020 2070 2e73 6574 4272           p.setBr
+00001d70: 7573 6828 5143 6f6c 6f72 2831 3934 2c20  ush(QColor(194, 
+00001d80: 3130 322c 2032 3139 2c20 3634 2929 0a20  102, 219, 64)). 
+00001d90: 2020 2020 2020 2020 2020 2070 2e73 6574             p.set
+00001da0: 5065 6e28 5143 6f6c 6f72 2831 3934 2c20  Pen(QColor(194, 
+00001db0: 3130 322c 2032 3139 2929 0a20 2020 2020  102, 219)).     
+00001dc0: 2020 2020 2020 2066 6f72 2063 6869 6c64         for child
+00001dd0: 2069 6e20 7365 6c66 2e73 656c 6563 7465   in self.selecte
+00001de0: 645f 6368 696c 6472 656e 3a0a 2020 2020  d_children:.    
+00001df0: 2020 2020 2020 2020 2020 2020 702e 6472              p.dr
+00001e00: 6177 5265 6374 280a 2020 2020 2020 2020  awRect(.        
+00001e10: 2020 2020 2020 2020 2020 2020 5152 6563              QRec
+00001e20: 7446 280a 2020 2020 2020 2020 2020 2020  tF(.            
+00001e30: 2020 2020 2020 2020 2020 2020 5150 6f69              QPoi
+00001e40: 6e74 4628 7365 6c66 2e67 6c78 5f74 6f5f  ntF(self.glx_to_
+00001e50: 6f76 6572 6c61 795f 7828 6368 696c 642e  overlay_x(child.
+00001e60: 6d69 6e5f 676c 7829 2c20 7365 6c66 2e67  min_glx), self.g
+00001e70: 6c79 5f74 6f5f 6f76 6572 6c61 795f 7928  ly_to_overlay_y(
+00001e80: 6368 696c 642e 6d69 6e5f 676c 7929 292c  child.min_gly)),
+00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ea0: 2020 2020 2020 2020 2051 506f 696e 7446           QPointF
+00001eb0: 2873 656c 662e 676c 785f 746f 5f6f 7665  (self.glx_to_ove
+00001ec0: 726c 6179 5f78 2863 6869 6c64 2e6d 6178  rlay_x(child.max
+00001ed0: 5f67 6c78 292c 2073 656c 662e 676c 795f  _glx), self.gly_
+00001ee0: 746f 5f6f 7665 726c 6179 5f79 2863 6869  to_overlay_y(chi
+00001ef0: 6c64 2e6d 6178 5f67 6c79 2929 0a20 2020  ld.max_gly)).   
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00001f20: 2020 2029 0a0a 2020 2020 2020 2020 702e     )..        p.
+00001f30: 7365 7450 656e 2851 742e 476c 6f62 616c  setPen(Qt.Global
+00001f40: 436f 6c6f 722e 7768 6974 6529 0a20 2020  Color.white).   
+00001f50: 2020 2020 2070 2e64 7261 7754 6578 7428       p.drawText(
+00001f60: 7265 6374 2c20 5174 2e41 6c69 676e 6d65  rect, Qt.Alignme
+00001f70: 6e74 466c 6167 2e41 6c69 676e 4c65 6674  ntFlag.AlignLeft
+00001f80: 207c 2051 742e 416c 6967 6e6d 656e 7446   | Qt.AlignmentF
+00001f90: 6c61 672e 416c 6967 6e54 6f70 2c20 275c  lag.AlignTop, '\
+00001fa0: 6e27 2e6a 6f69 6e28 7478 745f 6c69 7374  n'.join(txt_list
+00001fb0: 2929 0a                                  )).
```

### Comparing `janim-1.0.4/janim/imports.py` & `janim-1.1.0/janim/imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-'''
-使用 ``from janim.imports import *`` 即可导入 ``janim`` 主要的功能
-'''
-
-# flake8: noqa
-import janim.items.boolean_ops as boolean_ops
-from janim.anims.composition import *
-from janim.anims.creation import *
-from janim.anims.display import *
-from janim.anims.fading import *
-from janim.anims.growing import *
-from janim.anims.indication import *
-from janim.anims.rotation import *
-from janim.anims.timeline import *
-from janim.anims.transform import *
-from janim.anims.updater import *
-from janim.camera.camera import *
-from janim.camera.camera_info import *
-from janim.components.rgbas import apart_alpha, merge_alpha
-from janim.items.audio import *
-from janim.items.coordinate.coordinate_systems import *
-from janim.items.coordinate.functions import *
-from janim.items.coordinate.number_line import *
-from janim.items.geometry.arc import *
-from janim.items.geometry.arrow import *
-from janim.items.geometry.line import *
-from janim.items.geometry.polygon import *
-from janim.items.image_item import *
-from janim.items.item import *
-from janim.items.points import *
-from janim.items.shape_matchers import *
-from janim.items.svg.brace import *
-from janim.items.svg.svg_item import *
-from janim.items.svg.typst import *
-from janim.items.text.text import *
-from janim.items.value_tracker import *
-from janim.items.vitem import *
-from janim.utils.bezier import *
-from janim.utils.config import Config
-from janim.utils.file_ops import *
-from janim.utils.iterables import *
-from janim.utils.paths import *
-from janim.utils.rate_functions import *
-from janim.utils.simple_functions import *
-from janim.utils.space_ops import *
-from janim.exception import *
+'''
+使用 ``from janim.imports import *`` 即可导入 ``janim`` 主要的功能
+'''
+
+# flake8: noqa
+import janim.items.boolean_ops as boolean_ops
+from janim.anims.composition import *
+from janim.anims.creation import *
+from janim.anims.display import *
+from janim.anims.fading import *
+from janim.anims.growing import *
+from janim.anims.indication import *
+from janim.anims.movement import *
+from janim.anims.rotation import *
+from janim.anims.timeline import *
+from janim.anims.transform import *
+from janim.anims.updater import *
+from janim.camera.camera import *
+from janim.camera.camera_info import *
+from janim.components.rgbas import apart_alpha, merge_alpha
+from janim.exception import *
+from janim.items.audio import *
+from janim.items.coordinate.coordinate_systems import *
+from janim.items.coordinate.functions import *
+from janim.items.coordinate.number_line import *
+from janim.items.geometry.arc import *
+from janim.items.geometry.arrow import *
+from janim.items.geometry.line import *
+from janim.items.geometry.polygon import *
+from janim.items.image_item import *
+from janim.items.item import *
+from janim.items.points import *
+from janim.items.shape_matchers import *
+from janim.items.svg.brace import *
+from janim.items.svg.svg_item import *
+from janim.items.svg.typst import *
+from janim.items.text.text import *
+from janim.items.value_tracker import *
+from janim.items.vitem import *
+from janim.utils.bezier import *
+from janim.utils.config import Config
+from janim.utils.file_ops import *
+from janim.utils.iterables import *
+from janim.utils.paths import *
+from janim.utils.rate_functions import *
+from janim.utils.simple_functions import *
+from janim.utils.space_ops import *
```

### Comparing `janim-1.0.4/janim/items/boolean_ops.py` & `janim-1.1.0/janim/items/boolean_ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from __future__ import annotations
-
-import numpy as np
-import pathops
-
-from janim.exception import BooleanOpsError
-from janim.items.item import Item
-from janim.items.vitem import VItem
-from janim.utils.bezier import PathBuilder
-
-# Boolean operations between 2D mobjects
-# Borrowed from from https://github.com/ManimCommunity/manim/
-
-
-def _convert_vitem_to_skia_path(vitem: VItem) -> pathops.Path:
-    path = pathops.Path()
-    subpaths = vitem.points.get_subpaths()
-    for subpath in subpaths:
-        quads = vitem.points.get_bezier_tuples_from_points(subpath)
-        start = subpath[0]
-        path.moveTo(*start[:2])
-        for p0, p1, p2 in quads:
-            path.quadTo(*p1[:2], *p2[:2])
-        if np.isclose(subpath[0], subpath[-1]).all():
-            path.close()
-    return path
-
-
-def _convert_skia_path_to_vitem(
-    path: pathops.Path,
-    vitem: VItem
-) -> VItem:
-    PathVerb = pathops.PathVerb
-    builder: PathBuilder | None = None
-
-    for path_verb, points in path:
-        if path_verb == PathVerb.CLOSE:
-            builder.close_path()
-        else:
-            points = np.hstack((np.array(points), np.zeros((len(points), 1))))
-            if path_verb == PathVerb.MOVE:
-                for point in points:
-                    if builder is None:
-                        builder = PathBuilder(start_point=point)
-                    else:
-                        builder.move_to(point)
-            elif path_verb == PathVerb.CUBIC:
-                builder.cubic_to(*points)
-            elif path_verb == PathVerb.LINE:
-                builder.line_to(points[0])
-            elif path_verb == PathVerb.QUAD:
-                builder.conic_to(*points)
-            else:
-                raise BooleanOpsError(f'Unsupported: {path_verb}')
-
-    vitem.points.set([] if builder is None else builder.get()).reverse()
-    return vitem
-
-
-class Union(VItem):
-    '''
-    并集
-
-    传入两个及以上 :class:`~.VItem`，返回他它们区域的并集的外轮廓
-    '''
-    def __init__(self, *vitems: VItem, **kwargs):
-        if len(vitems) < 2:
-            raise BooleanOpsError("At least 2 items needed for Union.")
-        super().__init__(**kwargs)
-        outpen = pathops.Path()
-        pathops.union(
-            [
-                _convert_vitem_to_skia_path(vitem)
-                for vitem in vitems
-            ],
-            outpen.getPen()
-        )
-        _convert_skia_path_to_vitem(outpen, self)
-
-    @staticmethod
-    def from_item(item: Item, **kwargs) -> Union:
-        lst = [
-            sub
-            for sub in item.walk_self_and_descendants()
-            if isinstance(sub, VItem)
-        ]
-        return Union(*lst, **kwargs)
-
-
-class Difference(VItem):
-    '''
-    差集
-
-    传入 ``subitem`` 和 ``clip``，返回 ``subitem`` 裁去 ``clip`` 区域的轮廓线
-    '''
-    def __init__(self, subitem: VItem, clip: VItem, **kwargs):
-        super().__init__(**kwargs)
-        outpen = pathops.Path()
-        pathops.difference(
-            [_convert_vitem_to_skia_path(subitem)],
-            [_convert_vitem_to_skia_path(clip)],
-            outpen.getPen(),
-        )
-        _convert_skia_path_to_vitem(outpen, self)
-
-
-class Intersection(VItem):
-    '''
-    交集
-
-    传入两个及以上 :class:`~.VItem`，返回它们区域交集的外轮廓
-    '''
-    def __init__(self, *vitems: VItem, **kwargs):
-        if len(vitems) < 2:
-            raise BooleanOpsError("At least 2 items needed for Intersection.")
-        super().__init__(**kwargs)
-        outpen = pathops.Path()
-        pathops.intersection(
-            [_convert_vitem_to_skia_path(vitems[0])],
-            [_convert_vitem_to_skia_path(vitems[1])],
-            outpen.getPen(),
-        )
-        new_outpen = outpen
-        for _i in range(2, len(vitems)):
-            new_outpen = pathops.Path()
-            pathops.intersection(
-                [outpen],
-                [_convert_vitem_to_skia_path(vitems[_i])],
-                new_outpen.getPen(),
-            )
-            outpen = new_outpen
-        _convert_skia_path_to_vitem(outpen, self)
-
-    @staticmethod
-    def from_item(item: Item) -> Union:
-        lst = [
-            sub
-            for sub in item.walk_self_and_descendants()
-            if isinstance(sub, VItem)
-        ]
-        return Intersection(*lst)
-
-
-class Exclusion(VItem):
-    '''
-    补集
-
-    传入两个及以上 :class:`~.VItem`，返回它们的区域经过 XOR 运算后的外轮廓
-    '''
-    def __init__(self, *vitems: VItem, **kwargs):
-        if len(vitems) < 2:
-            raise BooleanOpsError("At least 2 items needed for Exclusion.")
-        super().__init__(**kwargs)
-        outpen = pathops.Path()
-        pathops.xor(
-            [_convert_vitem_to_skia_path(vitems[0])],
-            [_convert_vitem_to_skia_path(vitems[1])],
-            outpen.getPen(),
-        )
-        new_outpen = outpen
-        for _i in range(2, len(vitems)):
-            new_outpen = pathops.Path()
-            pathops.xor(
-                [outpen],
-                [_convert_vitem_to_skia_path(vitems[_i])],
-                new_outpen.getPen(),
-            )
-            outpen = new_outpen
-        _convert_skia_path_to_vitem(outpen, self)
+from __future__ import annotations
+
+import numpy as np
+import pathops
+
+from janim.exception import BooleanOpsError
+from janim.items.item import Item
+from janim.items.vitem import VItem
+from janim.utils.bezier import PathBuilder
+
+# Boolean operations between 2D items
+# Borrowed from from https://github.com/ManimCommunity/manim/
+
+
+def _convert_vitem_to_skia_path(vitem: VItem) -> pathops.Path:
+    path = pathops.Path()
+    subpaths = vitem.points.get_subpaths()
+    for subpath in subpaths:
+        quads = vitem.points.get_bezier_tuples_from_points(subpath)
+        start = subpath[0]
+        path.moveTo(*start[:2])
+        for p0, p1, p2 in quads:
+            path.quadTo(*p1[:2], *p2[:2])
+        if np.isclose(subpath[0], subpath[-1]).all():
+            path.close()
+    return path
+
+
+def _convert_skia_path_to_vitem(
+    path: pathops.Path,
+    vitem: VItem
+) -> VItem:
+    PathVerb = pathops.PathVerb
+    builder: PathBuilder | None = None
+
+    for path_verb, points in path:
+        if path_verb == PathVerb.CLOSE:
+            builder.close_path()
+        else:
+            points = np.hstack((np.array(points), np.zeros((len(points), 1))))
+            if path_verb == PathVerb.MOVE:
+                for point in points:
+                    if builder is None:
+                        builder = PathBuilder(start_point=point)
+                    else:
+                        builder.move_to(point)
+            elif path_verb == PathVerb.CUBIC:
+                builder.cubic_to(*points)
+            elif path_verb == PathVerb.LINE:
+                builder.line_to(points[0])
+            elif path_verb == PathVerb.QUAD:
+                builder.conic_to(*points)
+            else:
+                raise BooleanOpsError(f'Unsupported: {path_verb}')
+
+    vitem.points.set([] if builder is None else builder.get()).reverse()
+    return vitem
+
+
+class Union(VItem):
+    '''
+    并集
+
+    传入两个及以上 :class:`~.VItem`，返回他它们区域的并集的外轮廓
+    '''
+    def __init__(self, *vitems: VItem, **kwargs):
+        if len(vitems) < 2:
+            raise BooleanOpsError("At least 2 items needed for Union.")
+        super().__init__(**kwargs)
+        outpen = pathops.Path()
+        pathops.union(
+            [
+                _convert_vitem_to_skia_path(vitem)
+                for vitem in vitems
+            ],
+            outpen.getPen()
+        )
+        _convert_skia_path_to_vitem(outpen, self)
+
+    @staticmethod
+    def from_item(item: Item, **kwargs) -> Union:
+        lst = [
+            sub
+            for sub in item.walk_self_and_descendants()
+            if isinstance(sub, VItem)
+        ]
+        return Union(*lst, **kwargs)
+
+
+class Difference(VItem):
+    '''
+    差集
+
+    传入 ``subitem`` 和 ``clip``，返回 ``subitem`` 裁去 ``clip`` 区域的轮廓线
+    '''
+    def __init__(self, subitem: VItem, clip: VItem, **kwargs):
+        super().__init__(**kwargs)
+        outpen = pathops.Path()
+        pathops.difference(
+            [_convert_vitem_to_skia_path(subitem)],
+            [_convert_vitem_to_skia_path(clip)],
+            outpen.getPen(),
+        )
+        _convert_skia_path_to_vitem(outpen, self)
+
+
+class Intersection(VItem):
+    '''
+    交集
+
+    传入两个及以上 :class:`~.VItem`，返回它们区域交集的外轮廓
+    '''
+    def __init__(self, *vitems: VItem, **kwargs):
+        if len(vitems) < 2:
+            raise BooleanOpsError("At least 2 items needed for Intersection.")
+        super().__init__(**kwargs)
+        outpen = pathops.Path()
+        pathops.intersection(
+            [_convert_vitem_to_skia_path(vitems[0])],
+            [_convert_vitem_to_skia_path(vitems[1])],
+            outpen.getPen(),
+        )
+        new_outpen = outpen
+        for _i in range(2, len(vitems)):
+            new_outpen = pathops.Path()
+            pathops.intersection(
+                [outpen],
+                [_convert_vitem_to_skia_path(vitems[_i])],
+                new_outpen.getPen(),
+            )
+            outpen = new_outpen
+        _convert_skia_path_to_vitem(outpen, self)
+
+    @staticmethod
+    def from_item(item: Item) -> Union:
+        lst = [
+            sub
+            for sub in item.walk_self_and_descendants()
+            if isinstance(sub, VItem)
+        ]
+        return Intersection(*lst)
+
+
+class Exclusion(VItem):
+    '''
+    补集
+
+    传入两个及以上 :class:`~.VItem`，返回它们的区域经过 XOR 运算后的外轮廓
+    '''
+    def __init__(self, *vitems: VItem, **kwargs):
+        if len(vitems) < 2:
+            raise BooleanOpsError("At least 2 items needed for Exclusion.")
+        super().__init__(**kwargs)
+        outpen = pathops.Path()
+        pathops.xor(
+            [_convert_vitem_to_skia_path(vitems[0])],
+            [_convert_vitem_to_skia_path(vitems[1])],
+            outpen.getPen(),
+        )
+        new_outpen = outpen
+        for _i in range(2, len(vitems)):
+            new_outpen = pathops.Path()
+            pathops.xor(
+                [outpen],
+                [_convert_vitem_to_skia_path(vitems[_i])],
+                new_outpen.getPen(),
+            )
+            outpen = new_outpen
+        _convert_skia_path_to_vitem(outpen, self)
```

### Comparing `janim-1.0.4/janim/items/coordinate/coordinate_systems.py` & `janim-1.1.0/janim/items/coordinate/coordinate_systems.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,256 +1,257 @@
-
-from abc import ABCMeta, abstractmethod
-from typing import Callable, Iterable, Self, Sequence
-
-import numpy as np
-
-from janim.components.component import CmptInfo
-from janim.components.points import Cmpt_Points
-from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import (BLUE_D, DEGREES, DL, LEFT, ORIGIN, SMALL_BUFF,
-                             WHITE)
-from janim.items.coordinate.functions import ParametricCurve
-from janim.items.coordinate.number_line import NumberLine
-from janim.items.geometry.line import Line
-from janim.items.item import _ItemMeta
-from janim.items.points import Group
-from janim.items.vitem import DEFAULT_STROKE_RADIUS
-from janim.typing import RangeSpecifier, Vect
-from janim.utils.dict_ops import merge_dicts_recursively
-
-DEFAULT_X_RANGE = (-8.0, 8.0, 1.0)
-DEFAULT_Y_RANGE = (-4.0, 4.0, 1.0)
-
-
-class _ItemMeta_ABCMeta(_ItemMeta, ABCMeta):
-    pass
-
-
-class CoordinateSystem(metaclass=ABCMeta):
-    @staticmethod
-    def create_axis(
-        range: RangeSpecifier,
-        axis_config: dict,
-        length: float | None
-    ) -> NumberLine:
-        axis = NumberLine(range, width=length, **axis_config)
-        axis.points.shift(-axis.n2p(0))
-        return axis
-
-    @abstractmethod
-    def get_axes(self) -> list[NumberLine]:
-        pass
-
-    def coords_to_point(self, *coords: float | Iterable[float]) -> np.ndarray:
-        axes = self.get_axes()
-        origin = axes[0].number_to_point(0)
-        return origin + sum(
-            axis.number_to_point(coord) - origin
-            for axis, coord in zip(axes, coords)
-        )
-
-    def point_to_coords(self, point: Vect | Iterable[Vect]) -> np.ndarray:
-        raise NotImplementedError()     # TODO: point_to_coords
-
-    def c2p(self, *coords: float | np.ndarray) -> np.ndarray:
-        ''':meth:`coords_to_point` 的缩写'''
-        return self.coords_to_point(*coords)
-
-    def p2c(self, point: Vect | Iterable[Vect]) -> np.ndarray:
-        ''':meth:`point_to_coords` 的缩写'''
-        return self.point_to_coords(self, point)
-
-    def get_origin(self) -> np.ndarray:
-        return self.c2p(*[0] * len(self.get_axes()))
-
-
-class Axes(Group, CoordinateSystem, metaclass=_ItemMeta_ABCMeta):
-    axis_config_d: dict = dict(
-        numbers_to_exclude=[0]
-    )
-    x_axis_config_d: dict = {}
-    y_axis_config_d: dict = dict(
-        line_to_number_direction=LEFT
-    )
-
-    def __init__(
-        self,
-        x_range: RangeSpecifier = DEFAULT_X_RANGE,
-        y_range: RangeSpecifier = DEFAULT_Y_RANGE,
-        *,
-        num_sampled_graph_points_per_tick: int = 5,
-        axis_config: dict = {},
-        x_axis_config: dict = {},
-        y_axis_config: dict = {},
-        height: float | None = None,
-        width: float | None = None,
-        unit_size: float = 1.0,
-        **kwargs
-    ):
-        # REFACTOR: 将 num_sampled_graph_points_per_tick 提取到 CoordinateSystem 中？
-        CoordinateSystem.__init__(self)
-        self.x_range = x_range
-        self.y_range = y_range
-        self.num_sampled_graph_points_per_tick = num_sampled_graph_points_per_tick
-
-        axis_config = dict(**axis_config, unit_size=unit_size)
-        self.x_axis = self.create_axis(
-            x_range,
-            axis_config=merge_dicts_recursively(
-                self.axis_config_d,
-                self.x_axis_config_d,
-                axis_config,
-                x_axis_config
-            ),
-            length=width
-        )
-        self.y_axis = self.create_axis(
-            y_range,
-            axis_config=merge_dicts_recursively(
-                self.axis_config_d,
-                self.y_axis_config_d,
-                axis_config,
-                y_axis_config
-            ),
-            length=height
-        )
-        self.y_axis.points.rotate(90 * DEGREES, about_point=ORIGIN)
-
-        Group.__init__(self, self.x_axis, self.y_axis, **kwargs)
-
-    def get_axes(self) -> list[NumberLine]:
-        return [self.x_axis, self.y_axis]
-
-    def get_graph(
-        self,
-        function: Callable[[float], float],
-        x_range: Sequence[float] | None = None,
-        bind: bool = True,
-        **kwargs
-    ) -> ParametricCurve:
-        x_range = x_range or self.x_range
-        t_range = np.ones(3)
-        t_range[:len(x_range)] = x_range
-        # 对于坐标轴，x_range 的第三个元素是刻度步长
-        # 所以对于函数，需要除以 num_sampled_graph_points_per_tick
-        t_range[2] /= self.num_sampled_graph_points_per_tick
-
-        graph = ParametricCurve(
-            lambda t: self.c2p(t, function(t)),
-            t_range=tuple(t_range),
-            **kwargs
-        )
-
-        if bind:
-            Cmpt_Points.apply_points_fn.connect(
-                self.points,
-                lambda func, about_point: graph.points.apply_points_fn(func,
-                                                                       about_point=about_point,
-                                                                       about_edge=None)
-            )
-
-        return graph
-
-
-class CmptVPoints_NumberPlaneImpl(Cmpt_VPoints, impl=True):
-    def prepare_for_nonlinear_transform(self, num_inserted_curves: int = 50, *, root_only=False) -> Self:
-        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
-            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.has():
-                continue
-
-            curves_count = cmpt.curves_count()
-            if num_inserted_curves > curves_count:
-                cmpt.insert_n_curves(num_inserted_curves - curves_count)
-            cmpt.make_smooth_after_applying_functions = True
-
-        return self
-
-
-class NumberPlane(Axes):
-    points = CmptInfo(CmptVPoints_NumberPlaneImpl)
-
-    axis_config_d: dict = dict(
-        stroke_color=WHITE,
-        stroke_radius=0.01,
-        include_ticks=False,
-        include_tip=False,
-        line_to_number_buff=SMALL_BUFF,
-        line_to_number_direction=DL
-    )
-    y_axis_config_d: dict = dict(
-        line_to_number_direction=DL
-    )
-
-    def __init__(
-        self,
-        x_range: RangeSpecifier = DEFAULT_X_RANGE,
-        y_range: RangeSpecifier = DEFAULT_Y_RANGE,
-        background_line_style: dict = dict(
-            stroke_color=BLUE_D,
-            stroke_radius=0.01,
-        ),
-        # Defaults to a faded version of line_config
-        faded_line_style: dict = dict(),
-        faded_line_ratio: int = 4,
-        **kwargs
-    ):
-        super().__init__(
-            x_range,
-            y_range,
-            **kwargs
-        )
-        self.background_line_style = dict(background_line_style)
-        self.faded_line_style = dict(faded_line_style)
-        self.faded_line_ratio = faded_line_ratio
-        self._init_background_lines()
-
-    def _init_background_lines(self) -> None:
-        if not self.faded_line_style:
-            style = dict(self.background_line_style)
-
-            for key in ('fill_alpha', 'stroke_alpha', 'alpha'):
-                style[key] = 0.5 * style.get(key, 1)
-
-            style['stroke_radius'] = 0.5 * style.get('stroke_radius', DEFAULT_STROKE_RADIUS)
-
-            self.faded_line_style = style
-
-        x_lines1, x_lines2 = self.get_lines_parallel_to_axis(self.x_axis, self.y_axis)
-        y_lines1, y_lines2 = self.get_lines_parallel_to_axis(self.y_axis, self.x_axis)
-        self.background_lines = Group(*x_lines1, *y_lines1)
-        self.faded_lines = Group(*x_lines2, *y_lines2)
-
-        self.background_lines.digest_styles(**self.background_line_style)
-        self.faded_lines.digest_styles(**self.faded_line_style)
-
-        self.add(
-            self.faded_lines,
-            self.background_lines,
-            insert=True
-        )
-        self.depth.arrange()
-
-    def get_lines_parallel_to_axis(
-        self,
-        axis1: NumberLine,
-        axis2: NumberLine
-    ) -> tuple[Group, Group]:
-        freq = axis2.x_step
-        ratio = self.faded_line_ratio
-        line = Line(axis1.points.get_start(), axis1.points.get_end())
-        dense_freq = (1 + ratio)
-        step = (1 / dense_freq) * freq
-
-        lines1 = Group()
-        lines2 = Group()
-        inputs = np.arange(axis2.x_min, axis2.x_max + step, step)
-        for i, x in enumerate(inputs):
-            if abs(x) < 1e-8:
-                continue
-            new_line = line.copy()
-            new_line.points.shift(axis2.n2p(x) - axis2.n2p(0))
-            if i % (1 + ratio) == 0:
-                lines1.add(new_line)
-            else:
-                lines2.add(new_line)
-        return lines1, lines2
+
+from abc import ABCMeta, abstractmethod
+from typing import Callable, Iterable, Self, Sequence
+
+import numpy as np
+
+from janim.components.component import CmptInfo
+from janim.components.points import Cmpt_Points
+from janim.components.vpoints import Cmpt_VPoints
+from janim.constants import (BLUE_D, DEGREES, DL, LEFT, ORIGIN, SMALL_BUFF,
+                             WHITE)
+from janim.items.coordinate.functions import ParametricCurve
+from janim.items.coordinate.number_line import NumberLine
+from janim.items.geometry.line import Line
+from janim.items.item import _ItemMeta
+from janim.items.points import Group
+from janim.items.vitem import DEFAULT_STROKE_RADIUS
+from janim.typing import RangeSpecifier, Vect
+from janim.utils.dict_ops import merge_dicts_recursively
+
+DEFAULT_X_RANGE = (-8.0, 8.0, 1.0)
+DEFAULT_Y_RANGE = (-4.0, 4.0, 1.0)
+
+
+class _ItemMeta_ABCMeta(_ItemMeta, ABCMeta):
+    pass
+
+
+class CoordinateSystem(metaclass=ABCMeta):
+    @staticmethod
+    def create_axis(
+        range: RangeSpecifier,
+        axis_config: dict,
+        length: float | None
+    ) -> NumberLine:
+        axis = NumberLine(range, width=length, **axis_config)
+        axis.points.shift(-axis.n2p(0))
+        return axis
+
+    @abstractmethod
+    def get_axes(self) -> list[NumberLine]:
+        pass
+
+    def coords_to_point(self, *coords: float | Iterable[float]) -> np.ndarray:
+        axes = self.get_axes()
+        origin = axes[0].number_to_point(0)
+        return origin + sum(
+            axis.number_to_point(coord) - origin
+            for axis, coord in zip(axes, coords)
+        )
+
+    def point_to_coords(self, point: Vect | Iterable[Vect]) -> np.ndarray:
+        raise NotImplementedError()     # TODO: point_to_coords
+
+    def c2p(self, *coords: float | np.ndarray) -> np.ndarray:
+        ''':meth:`coords_to_point` 的缩写'''
+        return self.coords_to_point(*coords)
+
+    def p2c(self, point: Vect | Iterable[Vect]) -> np.ndarray:
+        ''':meth:`point_to_coords` 的缩写'''
+        return self.point_to_coords(self, point)
+
+    def get_origin(self) -> np.ndarray:
+        return self.c2p(*[0] * len(self.get_axes()))
+
+
+class Axes(Group, CoordinateSystem, metaclass=_ItemMeta_ABCMeta):
+    axis_config_d: dict = dict(
+        numbers_to_exclude=[0]
+    )
+    x_axis_config_d: dict = {}
+    y_axis_config_d: dict = dict(
+        line_to_number_direction=LEFT
+    )
+
+    def __init__(
+        self,
+        x_range: RangeSpecifier = DEFAULT_X_RANGE,
+        y_range: RangeSpecifier = DEFAULT_Y_RANGE,
+        *,
+        num_sampled_graph_points_per_tick: int = 5,
+        axis_config: dict = {},
+        x_axis_config: dict = {},
+        y_axis_config: dict = {},
+        height: float | None = None,
+        width: float | None = None,
+        unit_size: float = 1.0,
+        **kwargs
+    ):
+        # REFACTOR: 将 num_sampled_graph_points_per_tick 提取到 CoordinateSystem 中？
+        CoordinateSystem.__init__(self)
+        self.x_range = x_range
+        self.y_range = y_range
+        self.num_sampled_graph_points_per_tick = num_sampled_graph_points_per_tick
+
+        axis_config = dict(**axis_config, unit_size=unit_size)
+        self.x_axis = self.create_axis(
+            x_range,
+            axis_config=merge_dicts_recursively(
+                self.axis_config_d,
+                self.x_axis_config_d,
+                axis_config,
+                x_axis_config
+            ),
+            length=width
+        )
+        self.y_axis = self.create_axis(
+            y_range,
+            axis_config=merge_dicts_recursively(
+                self.axis_config_d,
+                self.y_axis_config_d,
+                axis_config,
+                y_axis_config
+            ),
+            length=height
+        )
+        self.y_axis.points.rotate(90 * DEGREES, about_point=ORIGIN)
+
+        Group.__init__(self, self.x_axis, self.y_axis, **kwargs)
+
+    def get_axes(self) -> list[NumberLine]:
+        return [self.x_axis, self.y_axis]
+
+    def get_graph(
+        self,
+        function: Callable[[float], float],
+        x_range: Sequence[float] | None = None,
+        bind: bool = True,
+        **kwargs
+    ) -> ParametricCurve:
+        x_range = x_range or self.x_range
+        t_range = np.ones(3)
+        t_range[:len(x_range)] = x_range
+        # 对于坐标轴，x_range 的第三个元素是刻度步长
+        # 所以对于函数，需要除以 num_sampled_graph_points_per_tick
+        t_range[2] /= self.num_sampled_graph_points_per_tick
+
+        graph = ParametricCurve(
+            lambda t: self.c2p(t, function(t)),
+            t_range=tuple(t_range),
+            **kwargs
+        )
+
+        if bind:
+            Cmpt_Points.apply_points_fn.connect(
+                self.points,
+                lambda func, about_point: graph.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
+            )
+
+        return graph
+
+
+class CmptVPoints_NumberPlaneImpl(Cmpt_VPoints, impl=True):
+    def prepare_for_nonlinear_transform(self, num_inserted_curves: int = 50, *, root_only=False) -> Self:
+        for cmpt in self.walk_same_cmpt_of_self_and_descendants_without_mock(root_only):
+            if not isinstance(cmpt, Cmpt_VPoints) or not cmpt.has():
+                continue
+
+            curves_count = cmpt.curves_count()
+            if num_inserted_curves > curves_count:
+                cmpt.insert_n_curves(num_inserted_curves - curves_count)
+            cmpt.make_smooth_after_applying_functions = True
+
+        return self
+
+
+class NumberPlane(Axes):
+    points = CmptInfo(CmptVPoints_NumberPlaneImpl)
+
+    background_line_style_d: dict = dict(
+        stroke_color=BLUE_D,
+        stroke_radius=0.01,
+    )
+    axis_config_d: dict = dict(
+        stroke_color=WHITE,
+        stroke_radius=0.01,
+        include_ticks=False,
+        include_tip=False,
+        line_to_number_buff=SMALL_BUFF,
+        line_to_number_direction=DL
+    )
+    y_axis_config_d: dict = dict(
+        line_to_number_direction=DL
+    )
+
+    def __init__(
+        self,
+        x_range: RangeSpecifier = DEFAULT_X_RANGE,
+        y_range: RangeSpecifier = DEFAULT_Y_RANGE,
+        background_line_style: dict = dict(),
+        # Defaults to a faded version of line_config
+        faded_line_style: dict = dict(),
+        faded_line_ratio: int = 4,
+        **kwargs
+    ):
+        super().__init__(
+            x_range,
+            y_range,
+            **kwargs
+        )
+        self.background_line_style = merge_dicts_recursively(self.background_line_style_d, background_line_style)
+        self.faded_line_style = dict(faded_line_style)
+        self.faded_line_ratio = faded_line_ratio
+        self._init_background_lines()
+
+    def _init_background_lines(self) -> None:
+        if not self.faded_line_style:
+            style = dict(self.background_line_style)
+
+            for key in ('fill_alpha', 'stroke_alpha', 'alpha'):
+                style[key] = 0.5 * style.get(key, 1)
+
+            style['stroke_radius'] = 0.5 * style.get('stroke_radius', DEFAULT_STROKE_RADIUS)
+
+            self.faded_line_style = style
+
+        x_lines1, x_lines2 = self.get_lines_parallel_to_axis(self.x_axis, self.y_axis)
+        y_lines1, y_lines2 = self.get_lines_parallel_to_axis(self.y_axis, self.x_axis)
+        self.background_lines = Group(*x_lines1, *y_lines1)
+        self.faded_lines = Group(*x_lines2, *y_lines2)
+
+        self.background_lines.digest_styles(**self.background_line_style)
+        self.faded_lines.digest_styles(**self.faded_line_style)
+
+        self.add(
+            self.faded_lines,
+            self.background_lines,
+            insert=True
+        )
+        self.depth.arrange()
+
+    def get_lines_parallel_to_axis(
+        self,
+        axis1: NumberLine,
+        axis2: NumberLine
+    ) -> tuple[Group, Group]:
+        freq = axis2.x_step
+        ratio = self.faded_line_ratio
+        line = Line(axis1.points.get_start(), axis1.points.get_end())
+        dense_freq = (1 + ratio)
+        step = (1 / dense_freq) * freq
+
+        lines1 = Group()
+        lines2 = Group()
+        inputs = np.arange(axis2.x_min, axis2.x_max + step, step)
+        for i, x in enumerate(inputs):
+            if abs(x) < 1e-8:
+                continue
+            new_line = line.copy()
+            new_line.points.shift(axis2.n2p(x) - axis2.n2p(0))
+            if i % (1 + ratio) == 0:
+                lines1.add(new_line)
+            else:
+                lines2.add(new_line)
+        return lines1, lines2
```

### Comparing `janim-1.0.4/janim/items/coordinate/functions.py` & `janim-1.1.0/janim/items/coordinate/functions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-
-from typing import Callable, Iterable
-
-import numpy as np
-
-from janim.constants import YELLOW
-from janim.items.vitem import VItem
-from janim.typing import JAnimColor, Vect
-from janim.utils.bezier import PathBuilder
-
-
-class ParametricCurve(VItem):
-    def __init__(
-        self,
-        t_func: Callable[[float], Vect],
-        t_range: tuple[float, float, float] = (0, 1, 0.1),
-        epsilon: float = 1e-8,
-        # TODO: automatically figure out discontinuities
-        discontinuities: Iterable[float] = [],
-        use_smoothing: bool = True,
-        **kwargs
-    ):
-        self.t_func = t_func
-        self.t_range = t_range
-        self.epsilon = epsilon
-        self.discontinuities = discontinuities
-        self.use_smoothing = use_smoothing
-
-        super().__init__(**kwargs)
-
-        t_min, t_max, step = t_range
-        builder = PathBuilder()
-
-        jumps = np.array(discontinuities)
-        jumps = jumps[(jumps > t_min) & (jumps < t_max)]
-        boundary_times = [t_min, t_max, *(jumps - epsilon), *(jumps + epsilon)]
-        boundary_times.sort()
-        for t1, t2 in zip(boundary_times[0::2], boundary_times[1::2]):
-            t_range = [*np.arange(t1, t2, step), t2]
-            points = np.array([t_func(t) for t in t_range])
-
-            builder.move_to(points[0])
-            for point in points[1:]:
-                builder.line_to(point)
-
-        self.points.set(builder.get())
-        if use_smoothing:
-            self.points.make_approximately_smooth()
-        if not self.points.has():
-            self.points.set(np.array([t_func(t_min)]))
-
-    def get_point_from_function(self, t: float) -> np.ndarray:
-        return np.array(self.t_func(t))
-
-
-class FunctionGraph(ParametricCurve):
-    def __init__(
-        self,
-        function: Callable[[float], float],
-        x_range: tuple[float, float, float] = (-8, 8, 0.25),
-        color: JAnimColor = YELLOW,
-        **kwargs
-    ):
-        super().__init__(
-            lambda t: [t, function(t), 0],
-            x_range,
-            color=color,
-            **kwargs
-        )
-
-
-# TODO: ImplicitFunction
+
+from typing import Callable, Iterable
+
+import numpy as np
+
+from janim.constants import YELLOW
+from janim.items.vitem import VItem
+from janim.typing import JAnimColor, Vect
+from janim.utils.bezier import PathBuilder
+
+
+class ParametricCurve(VItem):
+    def __init__(
+        self,
+        t_func: Callable[[float], Vect],
+        t_range: tuple[float, float, float] = (0, 1, 0.1),
+        epsilon: float = 1e-8,
+        # TODO: automatically figure out discontinuities
+        discontinuities: Iterable[float] = [],
+        use_smoothing: bool = True,
+        **kwargs
+    ):
+        self.t_func = t_func
+        self.t_range = t_range
+        self.epsilon = epsilon
+        self.discontinuities = discontinuities
+        self.use_smoothing = use_smoothing
+
+        super().__init__(**kwargs)
+
+        t_min, t_max, step = t_range
+        builder = PathBuilder()
+
+        jumps = np.array(discontinuities)
+        jumps = jumps[(jumps > t_min) & (jumps < t_max)]
+        boundary_times = [t_min, t_max, *(jumps - epsilon), *(jumps + epsilon)]
+        boundary_times.sort()
+        for t1, t2 in zip(boundary_times[0::2], boundary_times[1::2]):
+            t_range = [*np.arange(t1, t2, step), t2]
+            points = np.array([t_func(t) for t in t_range])
+
+            builder.move_to(points[0])
+            for point in points[1:]:
+                builder.line_to(point)
+
+        self.points.set(builder.get())
+        if use_smoothing:
+            self.points.make_approximately_smooth()
+        if not self.points.has():
+            self.points.set(np.array([t_func(t_min)]))
+
+    def get_point_from_function(self, t: float) -> np.ndarray:
+        return np.array(self.t_func(t))
+
+
+class FunctionGraph(ParametricCurve):
+    def __init__(
+        self,
+        function: Callable[[float], float],
+        x_range: tuple[float, float, float] = (-8, 8, 0.25),
+        color: JAnimColor = YELLOW,
+        **kwargs
+    ):
+        super().__init__(
+            lambda t: [t, function(t), 0],
+            x_range,
+            color=color,
+            **kwargs
+        )
+
+
+# TODO: ImplicitFunction
```

### Comparing `janim-1.0.4/janim/items/coordinate/number_line.py` & `janim-1.1.0/janim/items/coordinate/number_line.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-
-from typing import Iterable
-
-import numpy as np
-
-from janim.constants import DOWN, GREY_B, LEFT, MED_SMALL_BUFF, RIGHT, UP
-from janim.items.geometry.line import Line
-from janim.items.points import Group
-from janim.items.text.text import Text
-from janim.typing import JAnimColor, RangeSpecifier
-from janim.utils.bezier import interpolate, outer_interpolate
-from janim.utils.dict_ops import merge_dicts_recursively
-from janim.utils.simple_functions import fdiv
-
-
-class NumberLine(Line):
-    '''
-    数轴
-    '''
-
-    tip_config_d = dict(
-        back_width=0.25,
-        body_length=0.25
-    )
-    '''
-    箭头的默认属性
-    '''
-
-    decimal_number_config_d = dict(
-        num_decimal_places=0,
-        font_size=16
-    )
-    '''
-    数字的默认属性
-    '''
-
-    def __init__(
-        self,
-        x_range: RangeSpecifier = (-8, 8, 1),
-        *,
-        unit_size: int = 1,
-        color: JAnimColor = GREY_B,
-        stroke_radius: float = 0.01,
-        width: float | None = None,
-        include_tip: bool = False,                              # 是否显示箭头
-        tip_config: dict = {},                                  # 箭头属性
-        include_ticks: bool = True,                             # 是否显示刻度
-        tick_size: float = 0.1,                                 # 刻度大小
-        longer_tick_multiple: float = 1.5,                      # 长刻度大小倍数
-        numbers_with_elongated_ticks: Iterable[float] = [],     # 指定哪些数字是长刻度
-        include_numbers: bool = False,                          # 是否显示数字
-        numbers_to_exclude: Iterable[float] = [],               # 需要排除的数字
-        line_to_number_direction: np.ndarray = DOWN,            # 详见 get_number_item
-        line_to_number_buff: float = MED_SMALL_BUFF,            # 详见 get_number_item
-        decimal_number_config: dict = {},                       # 数字属性
-        **kwargs
-    ) -> None:
-        if len(x_range) == 2:
-            x_range = [*x_range, 1]
-        self.x_min, self.x_max, self.x_step = x_range
-
-        self.unit_size = unit_size
-
-        self.tip_config = merge_dicts_recursively(
-            self.tip_config_d,
-            tip_config
-        )
-
-        self.tick_size = tick_size
-        self.longer_tick_multiple = longer_tick_multiple
-
-        self.numbers_with_elongated_ticks = list(numbers_with_elongated_ticks)
-        self.numbers_to_exclude = list(numbers_to_exclude)
-        if include_tip:
-            self.numbers_to_exclude.append(self.x_max)
-
-        self.line_to_number_direction = line_to_number_direction
-        self.line_to_number_buff = line_to_number_buff
-
-        self.decimal_number_config = merge_dicts_recursively(
-            self.decimal_number_config_d,
-            decimal_number_config
-        )
-
-        super().__init__(
-            self.x_min * RIGHT, self.x_max * RIGHT,
-            color=color,
-            stroke_radius=stroke_radius,
-            **kwargs
-        )
-
-        if width:
-            self.points.set_width(width)
-            self.unit_size = self.get_unit_size()
-        else:
-            self.points.scale(self.unit_size)
-        self.points.to_center()
-
-        if include_tip:
-            self.add_tip(**self.tip_config)
-        if include_ticks:
-            self.add_ticks()
-        if include_numbers:
-            self.add_numbers()
-
-    def get_unit_size(self) -> float:
-        return self.points.length / (self.x_max - self.x_min)
-
-    def number_to_point(self, number: float | np.ndarray) -> np.ndarray:
-        alpha = (number - self.x_min) / (self.x_max - self.x_min)
-        return outer_interpolate(self.points.get_start(), self.points.get_end(), alpha)
-
-    def get_tick_range(self) -> np.ndarray:
-        tmp = self.x_min // self.x_step
-        mod = self.x_min % self.x_step
-        if mod >= 1e-5:
-            tmp += 1
-        x_min = self.x_step * tmp
-
-        tmp = self.x_max // self.x_step
-        mod = self.x_max % self.x_step
-        if self.x_step - mod < 1e-5:
-            tmp += 1.5
-        else:
-            tmp += 0.5
-        x_max = self.x_step * tmp
-
-        r = np.arange(x_min, x_max, self.x_step)
-        return r
-
-    def add_ticks(
-        self,
-        excluding: Iterable[float] | None = None,
-    ) -> None:
-        if excluding is None:
-            excluding = self.numbers_to_exclude
-
-        ticks = Group()
-        for x in self.get_tick_range():
-            if np.isclose(excluding, x).any():
-                continue
-
-            size = self.tick_size
-            if np.isclose(self.numbers_with_elongated_ticks, x).any():
-                size *= self.longer_tick_multiple
-            ticks.add(self.get_tick(x, size))
-        self.add(ticks)
-        self.ticks = ticks
-
-    def get_tick(self, x: float, size: float | None = None) -> Line:
-        if size is None:
-            size = self.tick_size
-        result = Line(size * DOWN, size * UP)
-        result.points.rotate(self.points.angle)
-        result.points.move_to(self.number_to_point(x))
-        result.stroke.set_rgbas([self.stroke.get()[0]])
-        return result
-
-    def add_numbers(
-        self,
-        x_values: Iterable[float] | None = None,
-        excluding: Iterable[float] | None = None,
-        font_size: int = 24,
-        **kwargs
-    ) -> Group:
-        if x_values is None:
-            x_values = self.get_tick_range()
-
-        if excluding is None:
-            excluding = self.numbers_to_exclude
-
-        numbers = Group()
-        for x in x_values:
-            if np.isclose(excluding, x).any():
-                continue
-            numbers.add(self.get_number_item(x, font_size=font_size, **kwargs))
-        self.add(numbers)
-        self.numbers = numbers
-        return numbers
-
-    def get_number_item(
-        self,
-        x: float,
-        direction: np.ndarray | None = None,
-        buff: float | None = None,
-        **number_config
-    ) -> Text:
-        number_config = self.decimal_number_config.copy()
-        number_config.update(number_config)
-
-        if direction is None:
-            direction = self.line_to_number_direction
-        if buff is None:
-            buff = self.line_to_number_buff
-
-        places = number_config.pop('num_decimal_places')
-
-        num_item = Text(str(round(x, places)), **number_config)
-        num_item.points.next_to(
-            self.number_to_point(x),
-            direction=direction,
-            buff=buff
-        )
-        if x < 0 and direction[0] == 0:
-            num_item.points.shift(num_item[0].points.box.width * LEFT / 2)
-        return num_item
-
-    def number_to_point(self, number: float | np.ndarray) -> np.ndarray:
-        alpha = (number - self.x_min) / (self.x_max - self.x_min)
-        return outer_interpolate(self.points.get_start(), self.points.get_end(), alpha)
-
-    def point_to_number(self, point: np.ndarray) -> float:
-        start = self.points.get_start()
-        end = self.points.get_end()
-        vect = end - start
-        proportion = fdiv(
-            np.dot(point - start, vect),
-            np.dot(end - start, vect),
-        )
-        return interpolate(self.x_min, self.x_max, proportion)
-
-    def n2p(self, number: float) -> np.ndarray:
-        '''``number_to_point`` 的缩写'''
-        return self.number_to_point(number)
-
-    def p2n(self, point: np.ndarray) -> float:
-        '''``point_to_number`` 的缩写'''
-        return self.point_to_number(point)
-
-
-class UnitInterval(NumberLine):
-    def __init__(
-        self,
-        x_range: RangeSpecifier = (0, 1, 0.1),
-        *,
-        unit_size: int = 10,
-        numbers_with_elongated_ticks: Iterable[float] = [0, 1],
-        decimal_number_config: dict = dict(
-            num_decimal_places=1
-        ),
-        **kwargs
-    ) -> None:
-        '''
-        单位长度数轴（0~1，分10段）
-        '''
-        super().__init__(
-            x_range,
-            unit_size=unit_size,
-            numbers_with_elongated_ticks=numbers_with_elongated_ticks,
-            decimal_number_config=decimal_number_config,
-            **kwargs
-        )
+
+from typing import Iterable
+
+import numpy as np
+
+from janim.constants import DOWN, GREY_B, LEFT, MED_SMALL_BUFF, RIGHT, UP
+from janim.items.geometry.line import Line
+from janim.items.points import Group
+from janim.items.text.text import Text
+from janim.typing import JAnimColor, RangeSpecifier
+from janim.utils.bezier import interpolate, outer_interpolate
+from janim.utils.dict_ops import merge_dicts_recursively
+from janim.utils.simple_functions import fdiv
+
+
+class NumberLine(Line):
+    '''
+    数轴
+    '''
+
+    tip_config_d = dict(
+        back_width=0.25,
+        body_length=0.25
+    )
+    '''
+    箭头的默认属性
+    '''
+
+    decimal_number_config_d = dict(
+        num_decimal_places=0,
+        font_size=16
+    )
+    '''
+    数字的默认属性
+    '''
+
+    def __init__(
+        self,
+        x_range: RangeSpecifier = (-8, 8, 1),
+        *,
+        unit_size: int = 1,
+        color: JAnimColor = GREY_B,
+        stroke_radius: float = 0.01,
+        width: float | None = None,
+        include_tip: bool = False,                              # 是否显示箭头
+        tip_config: dict = {},                                  # 箭头属性
+        include_ticks: bool = True,                             # 是否显示刻度
+        tick_size: float = 0.1,                                 # 刻度大小
+        longer_tick_multiple: float = 1.5,                      # 长刻度大小倍数
+        numbers_with_elongated_ticks: Iterable[float] = [],     # 指定哪些数字是长刻度
+        include_numbers: bool = False,                          # 是否显示数字
+        numbers_to_exclude: Iterable[float] = [],               # 需要排除的数字
+        line_to_number_direction: np.ndarray = DOWN,            # 详见 get_number_item
+        line_to_number_buff: float = MED_SMALL_BUFF,            # 详见 get_number_item
+        decimal_number_config: dict = {},                       # 数字属性
+        **kwargs
+    ) -> None:
+        if len(x_range) == 2:
+            x_range = [*x_range, 1]
+        self.x_min, self.x_max, self.x_step = x_range
+
+        self.unit_size = unit_size
+
+        self.tip_config = merge_dicts_recursively(
+            self.tip_config_d,
+            tip_config
+        )
+
+        self.tick_size = tick_size
+        self.longer_tick_multiple = longer_tick_multiple
+
+        self.numbers_with_elongated_ticks = list(numbers_with_elongated_ticks)
+        self.numbers_to_exclude = list(numbers_to_exclude)
+        if include_tip:
+            self.numbers_to_exclude.append(self.x_max)
+
+        self.line_to_number_direction = line_to_number_direction
+        self.line_to_number_buff = line_to_number_buff
+
+        self.decimal_number_config = merge_dicts_recursively(
+            self.decimal_number_config_d,
+            decimal_number_config
+        )
+
+        super().__init__(
+            self.x_min * RIGHT, self.x_max * RIGHT,
+            color=color,
+            stroke_radius=stroke_radius,
+            **kwargs
+        )
+
+        if width:
+            self.points.set_width(width)
+            self.unit_size = self.get_unit_size()
+        else:
+            self.points.scale(self.unit_size)
+        self.points.to_center()
+
+        if include_tip:
+            self.add_tip(**self.tip_config)
+        if include_ticks:
+            self.add_ticks()
+        if include_numbers:
+            self.add_numbers()
+
+    def get_unit_size(self) -> float:
+        return self.points.length / (self.x_max - self.x_min)
+
+    def number_to_point(self, number: float | np.ndarray) -> np.ndarray:
+        alpha = (number - self.x_min) / (self.x_max - self.x_min)
+        return outer_interpolate(self.points.get_start(), self.points.get_end(), alpha)
+
+    def get_tick_range(self) -> np.ndarray:
+        tmp = self.x_min // self.x_step
+        mod = self.x_min % self.x_step
+        if mod >= 1e-5:
+            tmp += 1
+        x_min = self.x_step * tmp
+
+        tmp = self.x_max // self.x_step
+        mod = self.x_max % self.x_step
+        if self.x_step - mod < 1e-5:
+            tmp += 1.5
+        else:
+            tmp += 0.5
+        x_max = self.x_step * tmp
+
+        r = np.arange(x_min, x_max, self.x_step)
+        return r
+
+    def add_ticks(
+        self,
+        excluding: Iterable[float] | None = None,
+    ) -> None:
+        if excluding is None:
+            excluding = self.numbers_to_exclude
+
+        ticks = Group()
+        for x in self.get_tick_range():
+            if np.isclose(excluding, x).any():
+                continue
+
+            size = self.tick_size
+            if np.isclose(self.numbers_with_elongated_ticks, x).any():
+                size *= self.longer_tick_multiple
+            ticks.add(self.get_tick(x, size))
+        self.add(ticks)
+        self.ticks = ticks
+
+    def get_tick(self, x: float, size: float | None = None) -> Line:
+        if size is None:
+            size = self.tick_size
+        result = Line(size * DOWN, size * UP)
+        result.points.rotate(self.points.angle)
+        result.points.move_to(self.number_to_point(x))
+        result.stroke.set_rgbas([self.stroke.get()[0]])
+        return result
+
+    def add_numbers(
+        self,
+        x_values: Iterable[float] | None = None,
+        excluding: Iterable[float] | None = None,
+        font_size: int = 24,
+        **kwargs
+    ) -> Group:
+        if x_values is None:
+            x_values = self.get_tick_range()
+
+        if excluding is None:
+            excluding = self.numbers_to_exclude
+
+        numbers = Group()
+        for x in x_values:
+            if np.isclose(excluding, x).any():
+                continue
+            numbers.add(self.get_number_item(x, font_size=font_size, **kwargs))
+        self.add(numbers)
+        self.numbers = numbers
+        return numbers
+
+    def get_number_item(
+        self,
+        x: float,
+        direction: np.ndarray | None = None,
+        buff: float | None = None,
+        **number_config
+    ) -> Text:
+        number_config = self.decimal_number_config.copy()
+        number_config.update(number_config)
+
+        if direction is None:
+            direction = self.line_to_number_direction
+        if buff is None:
+            buff = self.line_to_number_buff
+
+        places = number_config.pop('num_decimal_places')
+
+        num_item = Text(str(round(x, places)), **number_config)
+        num_item.points.next_to(
+            self.number_to_point(x),
+            direction=direction,
+            buff=buff
+        )
+        if x < 0 and direction[0] == 0:
+            num_item.points.shift(num_item[0].points.box.width * LEFT / 2)
+        return num_item
+
+    def number_to_point(self, number: float | np.ndarray) -> np.ndarray:
+        alpha = (number - self.x_min) / (self.x_max - self.x_min)
+        return outer_interpolate(self.points.get_start(), self.points.get_end(), alpha)
+
+    def point_to_number(self, point: np.ndarray) -> float:
+        start = self.points.get_start()
+        end = self.points.get_end()
+        vect = end - start
+        proportion = fdiv(
+            np.dot(point - start, vect),
+            np.dot(end - start, vect),
+        )
+        return interpolate(self.x_min, self.x_max, proportion)
+
+    def n2p(self, number: float) -> np.ndarray:
+        '''``number_to_point`` 的缩写'''
+        return self.number_to_point(number)
+
+    def p2n(self, point: np.ndarray) -> float:
+        '''``point_to_number`` 的缩写'''
+        return self.point_to_number(point)
+
+
+class UnitInterval(NumberLine):
+    def __init__(
+        self,
+        x_range: RangeSpecifier = (0, 1, 0.1),
+        *,
+        unit_size: int = 10,
+        numbers_with_elongated_ticks: Iterable[float] = [0, 1],
+        decimal_number_config: dict = dict(
+            num_decimal_places=1
+        ),
+        **kwargs
+    ) -> None:
+        '''
+        单位长度数轴（0~1，分10段）
+        '''
+        super().__init__(
+            x_range,
+            unit_size=unit_size,
+            numbers_with_elongated_ticks=numbers_with_elongated_ticks,
+            decimal_number_config=decimal_number_config,
+            **kwargs
+        )
```

### Comparing `janim-1.0.4/janim/items/geometry/arc.py` & `janim-1.1.0/janim/items/geometry/arc.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-
-from typing import Iterable, Self
-
-import numpy as np
-from janim.components.component import CmptInfo
-from janim.components.points import Cmpt_Points
-from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import LEFT, MED_SMALL_BUFF, NAN_POINT, ORIGIN, RIGHT, TAU
-from janim.items.item import Item
-from janim.items.vitem import VItem
-from janim.typing import Alpha, AlphaArray, Vect
-from janim.utils.bezier import PathBuilder, quadratic_bezier_points_for_arc
-from janim.utils.space_ops import (angle_between_vectors, angle_of_vector,
-                                   get_norm)
-
-DEFAULT_DOT_RADIUS = 0.08
-DEFAULT_SMALL_DOT_RADIUS = 0.04
-
-
-class ArcCenter(VItem):
-    '''
-    与圆弧有关的类的基类，被 :class:`Arc` 和 :class:`AnnularSector` 所继承
-    '''
-    _arc_center = CmptInfo(Cmpt_Points[Self])
-
-    def __init__(self, *args, arc_center: Vect = ORIGIN, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        self._arc_center.set([arc_center])
-
-        # 使 _arc_center 与 points 同步变换
-        Cmpt_VPoints.apply_points_fn.connect(
-            self.points,
-            lambda func, about_point: self._arc_center.apply_points_fn(func, about_point=about_point)
-        )
-
-    def get_arc_center(self) -> np.ndarray:
-        '''得到圆弧所对应的圆心'''
-        return self._arc_center.get()[0]
-
-    def move_arc_center_to(self, point: Vect) -> Self:
-        '''将圆弧圆心移动到指定的位置'''
-        self.points.shift(point - self.get_arc_center())
-        return self
-
-
-class Arc(ArcCenter):
-    '''
-    圆弧
-
-    - ``start_angle`` 表示起始的角度
-    - ``angle`` 表示圆心角
-    '''
-    _arc_center = CmptInfo(Cmpt_Points[Self])
-
-    def __init__(
-        self,
-        start_angle: float = 0,
-        angle: float = TAU / 4,
-        radius: float = 1.0,
-        *,
-        n_components: int = 8,
-        arc_center: np.ndarray = ORIGIN,
-        **kwargs
-    ) -> None:
-        super().__init__(arc_center=arc_center, **kwargs)
-
-        self.points.set(
-            quadratic_bezier_points_for_arc(
-                angle=angle,
-                start_angle=start_angle,
-                n_components=n_components
-            ) * radius + arc_center
-        )
-
-    def get_arc_length(self) -> float:
-        '''获取圆弧长度'''
-        center = self.get_arc_center()
-        p0 = self.points.get_start()
-        p1 = self.points.pfp(0.5)
-        vc0 = p0 - center
-        vc1 = p1 - center
-
-        return 2 * get_norm(vc0) * angle_between_vectors(vc0, vc1)
-
-    def get_start_angle(self) -> float:
-        '''获取起始角度'''
-        angle = angle_of_vector(self.points.get_start() - self.get_arc_center())
-        return angle % TAU
-
-    def get_stop_angle(self) -> float:
-        '''获取终止角度'''
-        angle = angle_of_vector(self.points.get_end() - self.get_arc_center())
-        return angle % TAU
-
-
-class ArcBetweenPoints(Arc):
-    '''
-    两点之间的圆弧
-
-    - 传入 ``start``, ``end`` 表示起点终点
-    - ``angle`` 表示圆心角
-    - 其余参数同 ``Arc``
-    '''
-    def __init__(
-        self,
-        start: np.ndarray,
-        end: np.ndarray,
-        angle: float = TAU / 4,
-        **kwargs
-    ) -> None:
-        super().__init__(angle=angle, **kwargs)
-        if angle == 0:
-            self.points.set_as_corners([LEFT, RIGHT])
-        self.points.put_start_and_end_on(start, end)
-
-
-class Cmpt_VPoints_CircleImpl[ItemT](Cmpt_VPoints[ItemT], impl=True):
-    '''
-    在圆中，对 :class:`~.Cmpt_VPoints` 的进一步实现
-    '''
-    def surround(
-        self,
-        item: Item,
-        dim_to_match: int = 0,
-        *,
-        stretch: bool = False,
-        buff: float = MED_SMALL_BUFF,
-        root_only: bool = True,
-        item_root_only: bool = False,
-    ) -> Self:
-        # Ignores dim_to_match and stretch; result will always be a circle
-        # REFACTOR:  Perhaps create an ellipse class to handle singele-dimension stretching
-        self.replace(item, dim_to_match, stretch=stretch, root_only=root_only, item_root_only=item_root_only)
-        self.set_size(self.box.width + 2 * buff, self.box.height + 2 * buff)
-        return self
-
-    @property
-    def start_angle(self) -> float:
-        '''获取起始角度'''
-        angle = angle_of_vector(self.get_start() - self.box.center)
-        return angle % TAU
-
-    def at_angle(self, angle: float) -> np.ndarray:
-        '''
-        得到在指定角度处的点，例如 ``angle=0`` 得到右侧的点，``angle=PI / 2`` 得到顶部的点
-        '''
-        return self.pfp(
-            (angle - self.start_angle) / TAU % 1
-        )
-
-    @property
-    def radius(self) -> float:
-        '''得到半径'''
-        return get_norm(self.get_start() - self.box.center)
-
-
-class Circle(VItem):
-    '''
-    圆
-
-    - 参数同 ``Arc``
-    - 半径传入 ``radius`` 指定
-    '''
-    points = CmptInfo(Cmpt_VPoints_CircleImpl[Self])
-
-    def __init__(
-        self,
-        radius: float = 1.0,
-        *,
-        n_components: int = 8,
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-
-        self.points.set(
-            quadratic_bezier_points_for_arc(
-                angle=TAU,
-                start_angle=0,
-                n_components=n_components
-            ) * radius
-        )
-
-
-class Dot(Circle):
-    '''
-    点，半径默认为 ``0.08``
-    '''
-    def __init__(
-        self,
-        point: np.ndarray = ORIGIN,
-        radius: float = DEFAULT_DOT_RADIUS,
-        *,
-        stroke_alpha: Alpha | AlphaArray | None = 0,
-        fill_alpha: Alpha | AlphaArray | None = 1.0,
-        **kwargs
-    ) -> None:
-        super().__init__(
-            radius=radius,
-            stroke_alpha=stroke_alpha,
-            fill_alpha=fill_alpha,
-            **kwargs
-        )
-        self.points.move_to(point)
-
-
-class SmallDot(Dot):
-    '''
-    小点，半径默认为 ``0.04``
-    '''
-    def __init__(self, *, radius: float = DEFAULT_SMALL_DOT_RADIUS, **kwargs) -> None:
-        super().__init__(radius=radius, **kwargs)
-
-
-class Ellipse(Circle):
-    '''
-    椭圆
-    '''
-    def __init__(
-        self,
-        width: float = 2,
-        height: float = 1,
-        **kwargs
-    ) -> None:
-        super().__init__(**kwargs)
-        self.points.set_size(width, height)
-
-
-class AnnularSector(ArcCenter):
-    '''
-    扇环
-
-    - ``inner_radius``: 内圆半径
-    - ``outer_radius``: 外圆半径
-    - ``start_angle``: 起始角度
-    - ``angle``: 圆心角
-    - ``arc_center``: 圆弧的中心
-    '''
-    def __init__(
-        self,
-        inner_radius: float = 0.5,
-        outer_radius: float = 1,
-        start_angle: float = 0,
-        angle: float = TAU / 4,
-        *,
-        arc_center: np.ndarray = ORIGIN,
-        n_components: int = 8,
-        **kwargs
-    ) -> None:
-        super().__init__(arc_center=arc_center, **kwargs)
-
-        unit = quadratic_bezier_points_for_arc(
-            angle=angle,
-            start_angle=start_angle,
-            n_components=n_components
-        )
-
-        inner_arc, outer_arc = (
-            unit * radius + arc_center
-            for radius in (inner_radius, outer_radius)
-        )
-        inner_arc = inner_arc[::-1]
-
-        builder = PathBuilder(points=outer_arc)
-        builder.append(inner_arc, line_to_start_point=True).close_path()
-
-        self.points.set(builder.get() + arc_center)
-
-
-class Sector(Arc):
-    '''
-    扇形
-
-    传入参数请参考 ``Arc``
-    '''
-    def __init__(self, *, arc_center: np.ndarray = ORIGIN, **kwargs) -> None:
-        super().__init__(arc_center=arc_center, **kwargs)
-
-        self.points.add_as_corners([arc_center, self.points.get_start()])
-
-
-class Annulus(VItem):
-    '''
-    圆环
-
-    - ``inner_radius``: 内圆半径
-    - ``outer_radius``: 外圆半径
-    - ``arc_center``: 圆弧的中心
-    '''
-    def __init__(
-        self,
-        outer_radius: float = 1,
-        inner_radius: float = 0.5,
-        *,
-        arc_center: np.ndarray = ORIGIN,
-        n_components: int = 8,
-        fill_alpha: float = 0.5,
-        **kwargs
-    ) -> None:
-        super().__init__(fill_alpha=fill_alpha, **kwargs)
-
-        unit = quadratic_bezier_points_for_arc(
-            TAU, 0,
-            n_components
-        )
-
-        inner, outer = (
-            unit * radius + arc_center
-            for radius in (inner_radius, outer_radius)
-        )
-        outer = outer[::-1]
-
-        self.points.set(np.vstack([outer, NAN_POINT, inner]))
+
+from typing import Iterable, Self
+
+import numpy as np
+from janim.components.component import CmptInfo
+from janim.components.points import Cmpt_Points
+from janim.components.vpoints import Cmpt_VPoints
+from janim.constants import LEFT, MED_SMALL_BUFF, NAN_POINT, ORIGIN, RIGHT, TAU
+from janim.items.item import Item
+from janim.items.vitem import VItem
+from janim.typing import Alpha, AlphaArray, Vect
+from janim.utils.bezier import PathBuilder, quadratic_bezier_points_for_arc
+from janim.utils.space_ops import (angle_between_vectors, angle_of_vector,
+                                   get_norm)
+
+DEFAULT_DOT_RADIUS = 0.08
+DEFAULT_SMALL_DOT_RADIUS = 0.04
+
+
+class ArcCenter(VItem):
+    '''
+    与圆弧有关的类的基类，被 :class:`Arc` 和 :class:`AnnularSector` 所继承
+    '''
+    _arc_center = CmptInfo(Cmpt_Points[Self])
+
+    def __init__(self, *args, arc_center: Vect = ORIGIN, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self._arc_center.set([arc_center])
+
+        # 使 _arc_center 与 points 同步变换
+        Cmpt_VPoints.apply_points_fn.connect(
+            self.points,
+            lambda func, about_point: self._arc_center.apply_points_fn(func, about_point=about_point)
+        )
+
+    def get_arc_center(self) -> np.ndarray:
+        '''得到圆弧所对应的圆心'''
+        return self._arc_center.get()[0]
+
+    def move_arc_center_to(self, point: Vect) -> Self:
+        '''将圆弧圆心移动到指定的位置'''
+        self.points.shift(point - self.get_arc_center())
+        return self
+
+
+class Arc(ArcCenter):
+    '''
+    圆弧
+
+    - ``start_angle`` 表示起始的角度
+    - ``angle`` 表示圆心角
+    '''
+    _arc_center = CmptInfo(Cmpt_Points[Self])
+
+    def __init__(
+        self,
+        start_angle: float = 0,
+        angle: float = TAU / 4,
+        radius: float = 1.0,
+        *,
+        n_components: int = 8,
+        arc_center: np.ndarray = ORIGIN,
+        **kwargs
+    ) -> None:
+        super().__init__(arc_center=arc_center, **kwargs)
+
+        self.points.set(
+            quadratic_bezier_points_for_arc(
+                angle=angle,
+                start_angle=start_angle,
+                n_components=n_components
+            ) * radius + arc_center
+        )
+
+    def get_arc_length(self) -> float:
+        '''获取圆弧长度'''
+        center = self.get_arc_center()
+        p0 = self.points.get_start()
+        p1 = self.points.pfp(0.5)
+        vc0 = p0 - center
+        vc1 = p1 - center
+
+        return 2 * get_norm(vc0) * angle_between_vectors(vc0, vc1)
+
+    def get_start_angle(self) -> float:
+        '''获取起始角度'''
+        angle = angle_of_vector(self.points.get_start() - self.get_arc_center())
+        return angle % TAU
+
+    def get_stop_angle(self) -> float:
+        '''获取终止角度'''
+        angle = angle_of_vector(self.points.get_end() - self.get_arc_center())
+        return angle % TAU
+
+
+class ArcBetweenPoints(Arc):
+    '''
+    两点之间的圆弧
+
+    - 传入 ``start``, ``end`` 表示起点终点
+    - ``angle`` 表示圆心角
+    - 其余参数同 ``Arc``
+    '''
+    def __init__(
+        self,
+        start: np.ndarray,
+        end: np.ndarray,
+        angle: float = TAU / 4,
+        **kwargs
+    ) -> None:
+        super().__init__(angle=angle, **kwargs)
+        if angle == 0:
+            self.points.set_as_corners([LEFT, RIGHT])
+        self.points.put_start_and_end_on(start, end)
+
+
+class Cmpt_VPoints_CircleImpl[ItemT](Cmpt_VPoints[ItemT], impl=True):
+    '''
+    在圆中，对 :class:`~.Cmpt_VPoints` 的进一步实现
+    '''
+    def surround(
+        self,
+        item: Item,
+        dim_to_match: int = 0,
+        *,
+        stretch: bool = False,
+        buff: float = MED_SMALL_BUFF,
+        root_only: bool = True,
+        item_root_only: bool = False,
+    ) -> Self:
+        # Ignores dim_to_match and stretch; result will always be a circle
+        # REFACTOR:  Perhaps create an ellipse class to handle singele-dimension stretching
+        self.replace(item, dim_to_match, stretch=stretch, root_only=root_only, item_root_only=item_root_only)
+        self.set_size(self.box.width + 2 * buff, self.box.height + 2 * buff)
+        return self
+
+    @property
+    def start_angle(self) -> float:
+        '''获取起始角度'''
+        angle = angle_of_vector(self.get_start() - self.box.center)
+        return angle % TAU
+
+    def at_angle(self, angle: float) -> np.ndarray:
+        '''
+        得到在指定角度处的点，例如 ``angle=0`` 得到右侧的点，``angle=PI / 2`` 得到顶部的点
+        '''
+        return self.pfp(
+            (angle - self.start_angle) / TAU % 1
+        )
+
+    @property
+    def radius(self) -> float:
+        '''得到半径'''
+        return get_norm(self.get_start() - self.box.center)
+
+
+class Circle(VItem):
+    '''
+    圆
+
+    - 参数同 ``Arc``
+    - 半径传入 ``radius`` 指定
+    '''
+    points = CmptInfo(Cmpt_VPoints_CircleImpl[Self])
+
+    def __init__(
+        self,
+        radius: float = 1.0,
+        *,
+        n_components: int = 8,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+
+        self.points.set(
+            quadratic_bezier_points_for_arc(
+                angle=TAU,
+                start_angle=0,
+                n_components=n_components
+            ) * radius
+        )
+
+
+class Dot(Circle):
+    '''
+    点，半径默认为 ``0.08``
+    '''
+    def __init__(
+        self,
+        point: np.ndarray = ORIGIN,
+        radius: float = DEFAULT_DOT_RADIUS,
+        *,
+        stroke_alpha: Alpha | AlphaArray | None = 0,
+        fill_alpha: Alpha | AlphaArray | None = 1.0,
+        **kwargs
+    ) -> None:
+        super().__init__(
+            radius=radius,
+            stroke_alpha=stroke_alpha,
+            fill_alpha=fill_alpha,
+            **kwargs
+        )
+        self.points.move_to(point)
+
+
+class SmallDot(Dot):
+    '''
+    小点，半径默认为 ``0.04``
+    '''
+    def __init__(self, *, radius: float = DEFAULT_SMALL_DOT_RADIUS, **kwargs) -> None:
+        super().__init__(radius=radius, **kwargs)
+
+
+class Ellipse(Circle):
+    '''
+    椭圆
+    '''
+    def __init__(
+        self,
+        width: float = 2,
+        height: float = 1,
+        **kwargs
+    ) -> None:
+        super().__init__(**kwargs)
+        self.points.set_size(width, height)
+
+
+class AnnularSector(ArcCenter):
+    '''
+    扇环
+
+    - ``inner_radius``: 内圆半径
+    - ``outer_radius``: 外圆半径
+    - ``start_angle``: 起始角度
+    - ``angle``: 圆心角
+    - ``arc_center``: 圆弧的中心
+    '''
+    def __init__(
+        self,
+        inner_radius: float = 0.5,
+        outer_radius: float = 1,
+        start_angle: float = 0,
+        angle: float = TAU / 4,
+        *,
+        arc_center: np.ndarray = ORIGIN,
+        n_components: int = 8,
+        **kwargs
+    ) -> None:
+        super().__init__(arc_center=arc_center, **kwargs)
+
+        unit = quadratic_bezier_points_for_arc(
+            angle=angle,
+            start_angle=start_angle,
+            n_components=n_components
+        )
+
+        inner_arc, outer_arc = (
+            unit * radius + arc_center
+            for radius in (inner_radius, outer_radius)
+        )
+        inner_arc = inner_arc[::-1]
+
+        builder = PathBuilder(points=outer_arc)
+        builder.append(inner_arc, line_to_start_point=True).close_path()
+
+        self.points.set(builder.get() + arc_center)
+
+
+class Sector(Arc):
+    '''
+    扇形
+
+    传入参数请参考 ``Arc``
+    '''
+    def __init__(self, *, arc_center: np.ndarray = ORIGIN, **kwargs) -> None:
+        super().__init__(arc_center=arc_center, **kwargs)
+
+        self.points.add_as_corners([arc_center, self.points.get_start()])
+
+
+class Annulus(VItem):
+    '''
+    圆环
+
+    - ``inner_radius``: 内圆半径
+    - ``outer_radius``: 外圆半径
+    - ``arc_center``: 圆弧的中心
+    '''
+    def __init__(
+        self,
+        outer_radius: float = 1,
+        inner_radius: float = 0.5,
+        *,
+        arc_center: np.ndarray = ORIGIN,
+        n_components: int = 8,
+        fill_alpha: float = 0.5,
+        **kwargs
+    ) -> None:
+        super().__init__(fill_alpha=fill_alpha, **kwargs)
+
+        unit = quadratic_bezier_points_for_arc(
+            TAU, 0,
+            n_components
+        )
+
+        inner, outer = (
+            unit * radius + arc_center
+            for radius in (inner_radius, outer_radius)
+        )
+        outer = outer[::-1]
+
+        self.points.set(np.vstack([outer, NAN_POINT, inner]))
```

### Comparing `janim-1.0.4/janim/items/geometry/arrow.py` & `janim-1.1.0/janim/items/geometry/arrow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,227 @@
-from __future__ import annotations
-
-from enum import Enum
-from typing import Self
-
-import numpy as np
-
-from janim.constants import DOWN, LEFT, ORIGIN, RIGHT, UP, np
-from janim.items.geometry.line import Line
-from janim.items.vitem import DEFAULT_STROKE_RADIUS, VItem
-from janim.utils.space_ops import (get_norm, midpoint, normalize,
-                                   rotation_between_vectors)
-
-DEFAULT_ARROWTIP_BODY_LENGTH = 0.2
-DEFAULT_ARROWTIP_BACK_WIDTH = 0.2
-
-
-class CenterAnchor(Enum):
-    '''
-    箭头原点所处位置的选项
-
-    图形示意：
-
-    .. code-block:: text
-
-        .-----
-        |        -----
-        |               -----
-        [Back]  [Center]  [Front]
-        |               -----
-        |        -----
-        .-----
-    '''
-    Back = 0
-    Center = 1
-    Front = 2
-
-
-class ArrowTip(VItem):
-    '''
-    箭头标志
-
-    - ``body_length``: 箭头的宽度
-    - ``back_width``: 箭头的长度
-    - ``center_anchor``: 原点所处的位置，请参考 :class:`CenterAnchor`
-    '''
-
-    def __init__(   # TODO: 3d-ops
-        self,
-        body_length: float = DEFAULT_ARROWTIP_BODY_LENGTH,
-        back_width: float = DEFAULT_ARROWTIP_BACK_WIDTH,
-        angle: float = 0,
-        *,
-        center_anchor: CenterAnchor = CenterAnchor.Back,
-        fill_alpha: float = 1.0,
-        stroke_radius: float = DEFAULT_STROKE_RADIUS / 4,
-        **kwargs
-    ) -> None:
-        super().__init__(fill_alpha=fill_alpha, stroke_radius=stroke_radius, **kwargs)
-        self.center_anchor = center_anchor
-
-        self.points.set_as_corners([
-            body_length * RIGHT,
-            back_width / 2 * UP,
-            back_width / 2 * DOWN,
-            body_length * RIGHT
-        ])
-        self.points.to_center()
-        self.rotate_about_anchor(angle)
-
-    def get_center_anchor(self) -> np.ndarray:
-        '''
-        根据设定的 ``center_anchor`` 得到原点位置，
-        请参考 :class:`ArrowTip.CenterAnchor`
-        '''
-        points = self.points._points.data
-        if self.center_anchor == CenterAnchor.Back:
-            return points[3]
-        if self.center_anchor == CenterAnchor.Center:
-            return midpoint(points[0], points[3])
-        # if self.center_anchor == CenterAnchor.Front:
-        return points[0]
-
-    @property
-    def direction(self) -> np.ndarray:
-        '''得到箭头的方向（单位向量）'''
-        points = self.points._points.data
-        return normalize(points[0] - points[3])
-
-    @property
-    def body_length(self) -> float:
-        '''得到箭头的长度'''
-        points = self.points._points.data
-        return get_norm(points[0] - points[3])
-
-    @property
-    def back_width(self) -> float:
-        '''得到箭头的宽度'''
-        points = self.points._points.data
-        return get_norm(points[4] - points[2])
-
-    def rotate_about_anchor(self, angle: float) -> Self:
-        '''相对于原点位置进行旋转'''
-        self.points.rotate(angle, about_point=self.get_center_anchor())
-
-    def move_anchor_to(self, pos: np.ndarray) -> Self:
-        '''将原点移动到指定位置'''
-        self.points.shift(pos - self.get_center_anchor())
-        return self
-
-
-class Arrow(Line):
-    '''
-    带箭头的线段，箭头大小自动
-
-    - ``buff``: 箭头首尾的空余量，默认为 ``0.25``
-    - ``max_length_to_tip_length_ratio``: 箭头长度和直线长度最大比例
-    '''
-    def __init__(
-        self,
-        start: np.ndarray = LEFT,
-        end: np.ndarray = RIGHT,
-        *,
-        buff: float = 0.25,
-        max_length_to_tip_length_ratio: float | None = 0.3,
-        tip_kwargs: dict = {},
-        **kwargs
-    ) -> None:
-        if 'center_anchor' not in tip_kwargs:
-            tip_kwargs['center_anchor'] = CenterAnchor.Center
-
-        super().__init__(start, end, buff=buff, **kwargs)
-        self.max_length_to_tip_length_ratio = max_length_to_tip_length_ratio
-
-        self.init_tips(tip_kwargs)
-        self.place_tip()
-
-    def init_tips(self, tip_kwargs: dict) -> None:
-        self.tip = self.add_tip(**tip_kwargs)
-        self.tip_orig_body_length = self.tip.body_length
-
-    def copy(self, *, root_only=False) -> Self:
-        copy_item = super().copy(root_only=root_only)
-        if root_only:
-            copy_item.tip = None
-        else:
-            copy_item.tip = copy_item[0]
-        return copy_item
-
-    def _place_tip(
-        self,
-        tip: ArrowTip,
-        target: np.ndarray,
-        target_direction: np.ndarray
-    ) -> None:
-        direction = tip.direction
-
-        length = self.tip_orig_body_length
-
-        if self.max_length_to_tip_length_ratio:
-            max_length = self.points.arc_length * self.max_length_to_tip_length_ratio
-            length = min(length, max_length)
-
-        min_length = self.radius.get()[0] * 2 * self.tip.body_length / self.tip.back_width
-        length = max(length, min_length)
-
-        scale_factor = length / tip.body_length
-
-        tip.points.scale(scale_factor)
-        if not np.isclose(direction, target_direction).all():
-            tip.points.apply_matrix(rotation_between_vectors(direction, target_direction))
-        tip.move_anchor_to(target)
-
-    def place_tip(self) -> Self:
-        self._place_tip(self.tip, self.points.get_end(), self.points.end_direction)
-        return self
-
-
-class Vector(Arrow):
-    '''
-    起点为 ORIGIN 的箭头，终点为 ``direction``
-
-    - ``buff`` 默认设为了 0
-    '''
-    def __init__(self, direction: np.ndarray = RIGHT, *, buff: float = 0, **kwargs):
-        if len(direction) == 2:
-            direction = np.hstack([direction, 0])
-        super().__init__(ORIGIN, direction, buff=buff, **kwargs)
-
-
-class DoubleArrow(Arrow):
-    '''
-    双向箭头
-
-    参数请参考 :class:`Arrow`
-    '''
-    def __init__(self, *args, tip_kwargs: dict = {}, **kwargs) -> None:
-        super().__init__(*args, tip_kwargs=tip_kwargs, **kwargs)
-
-    def init_tips(self, tip_kwargs: dict) -> None:
-        super().init_tips(tip_kwargs)
-        self.start_tip = self.add_tip(0, True, **tip_kwargs)
-
-    def copy(self, *, root_only=False) -> Self:
-        copy_item = super().copy(root_only=root_only)
-        if root_only:
-            copy_item.start_tip = None
-        else:
-            copy_item.start_tip = copy_item[1]
-        return copy_item
-
-    def place_tip(self) -> Self:
-        super().place_tip()
-        self._place_tip(self.start_tip, self.points.get_start(), -self.points.start_direction)
-        return self
-
-
-# TODO: FillArrow
+from __future__ import annotations
+
+from enum import Enum
+from typing import Self
+
+import numpy as np
+
+from janim.constants import DOWN, LEFT, ORIGIN, RIGHT, UP, np
+from janim.items.geometry.line import Line
+from janim.items.vitem import DEFAULT_STROKE_RADIUS, VItem
+from janim.utils.space_ops import (get_norm, midpoint, normalize,
+                                   rotation_between_vectors)
+
+DEFAULT_ARROWTIP_BODY_LENGTH = 0.2
+DEFAULT_ARROWTIP_BACK_WIDTH = 0.2
+
+
+class CenterAnchor(Enum):
+    '''
+    箭头原点所处位置的选项
+
+    图形示意：
+
+    .. code-block:: text
+
+        .-----
+        |        -----
+        |               -----
+        [Back]  [Center]  [Front]
+        |               -----
+        |        -----
+        .-----
+    '''
+    Back = 0
+    Center = 1
+    Front = 2
+
+
+class ArrowTip(VItem):
+    '''
+    箭头标志
+
+    - ``body_length``: 箭头的宽度
+    - ``back_width``: 箭头的长度
+    - ``center_anchor``: 原点所处的位置，请参考 :class:`CenterAnchor`
+    '''
+
+    def __init__(   # TODO: 3d-ops
+        self,
+        body_length: float = DEFAULT_ARROWTIP_BODY_LENGTH,
+        back_width: float = DEFAULT_ARROWTIP_BACK_WIDTH,
+        angle: float = 0,
+        *,
+        center_anchor: CenterAnchor = CenterAnchor.Back,
+        fill_alpha: float = 1.0,
+        stroke_radius: float = DEFAULT_STROKE_RADIUS / 4,
+        **kwargs
+    ) -> None:
+        super().__init__(fill_alpha=fill_alpha, stroke_radius=stroke_radius, **kwargs)
+        self.center_anchor = center_anchor
+
+        self.points.set_as_corners([
+            body_length * RIGHT,
+            back_width / 2 * UP,
+            back_width / 2 * DOWN,
+            body_length * RIGHT
+        ])
+        self.points.to_center()
+        self.rotate_about_anchor(angle)
+
+    def get_center_anchor(self) -> np.ndarray:
+        '''
+        根据设定的 ``center_anchor`` 得到原点位置，
+        请参考 :class:`ArrowTip.CenterAnchor`
+        '''
+        points = self.points._points.data
+        if self.center_anchor == CenterAnchor.Back:
+            return points[3]
+        if self.center_anchor == CenterAnchor.Center:
+            return midpoint(points[0], points[3])
+        # if self.center_anchor == CenterAnchor.Front:
+        return points[0]
+
+    @property
+    def direction(self) -> np.ndarray:
+        '''得到箭头的方向（单位向量）'''
+        points = self.points._points.data
+        return normalize(points[0] - points[3])
+
+    @property
+    def body_length(self) -> float:
+        '''得到箭头的长度'''
+        points = self.points._points.data
+        return get_norm(points[0] - points[3])
+
+    @property
+    def back_width(self) -> float:
+        '''得到箭头的宽度'''
+        points = self.points._points.data
+        return get_norm(points[4] - points[2])
+
+    def rotate_about_anchor(self, angle: float) -> Self:
+        '''相对于原点位置进行旋转'''
+        self.points.rotate(angle, about_point=self.get_center_anchor())
+
+    def move_anchor_to(self, pos: np.ndarray) -> Self:
+        '''将原点移动到指定位置'''
+        self.points.shift(pos - self.get_center_anchor())
+        return self
+
+
+class Arrow(Line):
+    '''
+    带箭头的线段，箭头大小自动
+
+    - ``buff``: 箭头首尾的空余量，默认为 ``0.25``
+    - ``max_length_to_tip_length_ratio``: 箭头长度和直线长度最大比例
+    '''
+    def __init__(
+        self,
+        start: np.ndarray = LEFT,
+        end: np.ndarray = RIGHT,
+        *,
+        buff: float = 0.25,
+        max_length_to_tip_length_ratio: float | None = 0.3,
+        tip_kwargs: dict = {},
+        **kwargs
+    ) -> None:
+        if 'center_anchor' not in tip_kwargs:
+            tip_kwargs['center_anchor'] = CenterAnchor.Center
+
+        super().__init__(start, end, buff=buff, **kwargs)
+        self.max_length_to_tip_length_ratio = max_length_to_tip_length_ratio
+
+        self.init_tips(tip_kwargs)
+        self.place_tip()
+
+    def init_tips(self, tip_kwargs: dict) -> None:
+        self.tip = self.add_tip(**tip_kwargs)
+        self.tip_orig_body_length = self.tip.body_length
+
+    def copy(self, *, root_only=False) -> Self:
+        copy_item = super().copy(root_only=root_only)
+        if root_only:
+            copy_item.tip = None
+        else:
+            copy_item.tip = copy_item[0]
+        return copy_item
+
+    def _place_tip(
+        self,
+        tip: ArrowTip,
+        target: np.ndarray,
+        target_direction: np.ndarray
+    ) -> None:
+        direction = tip.direction
+
+        length = self.tip_orig_body_length
+
+        if self.max_length_to_tip_length_ratio:
+            max_length = self.points.arc_length * self.max_length_to_tip_length_ratio
+            length = min(length, max_length)
+
+        min_length = self.radius.get()[0] * 2 * self.tip.body_length / self.tip.back_width
+        length = max(length, min_length)
+
+        scale_factor = length / tip.body_length
+
+        tip.points.scale(scale_factor)
+        if not np.isclose(direction, target_direction).all():
+            tip.points.apply_matrix(rotation_between_vectors(direction, target_direction))
+        tip.move_anchor_to(target)
+
+    def place_tip(self) -> Self:
+        self._place_tip(self.tip, self.points.get_end(), self.points.end_direction)
+        return self
+
+
+class Vector(Arrow):
+    '''
+    起点为 ORIGIN 的箭头，终点为 ``direction``
+
+    - ``buff`` 默认设为了 0
+    '''
+    def __init__(
+        self,
+        direction: np.ndarray = RIGHT,
+        *,
+        buff: float = 0,
+        tip_kwargs: dict = {},
+        **kwargs
+    ):
+        tip_kwargs.setdefault('center_anchor', CenterAnchor.Front)
+
+        if len(direction) == 2:
+            direction = np.hstack([direction, 0])
+        super().__init__(ORIGIN, direction, buff=buff, tip_kwargs=tip_kwargs, **kwargs)
+
+
+class DoubleArrow(Arrow):
+    '''
+    双向箭头
+
+    参数请参考 :class:`Arrow`
+    '''
+    def __init__(self, *args, tip_kwargs: dict = {}, **kwargs) -> None:
+        super().__init__(*args, tip_kwargs=tip_kwargs, **kwargs)
+
+    def init_tips(self, tip_kwargs: dict) -> None:
+        super().init_tips(tip_kwargs)
+        self.start_tip = self.add_tip(0, True, **tip_kwargs)
+
+    def copy(self, *, root_only=False) -> Self:
+        copy_item = super().copy(root_only=root_only)
+        if root_only:
+            copy_item.start_tip = None
+        else:
+            copy_item.start_tip = copy_item[1]
+        return copy_item
+
+    def place_tip(self) -> Self:
+        super().place_tip()
+        self._place_tip(self.start_tip, self.points.get_start(), -self.points.start_direction)
+        return self
+
+
+# TODO: FillArrow
```

### Comparing `janim-1.0.4/janim/items/geometry/line.py` & `janim-1.1.0/janim/items/geometry/line.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-from __future__ import annotations
-
-import math
-from typing import Self
-
-import numpy as np
-
-from janim.components.component import CmptInfo
-from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import LEFT, ORIGIN, RIGHT, UP
-from janim.items.points import Points
-from janim.items.vitem import VItem
-from janim.typing import Vect
-from janim.utils.bezier import PathBuilder
-from janim.utils.simple_functions import clip
-from janim.utils.space_ops import angle_of_vector, get_norm, normalize
-
-type SupportsPointify = Vect | Points
-
-
-class Cmpt_VPoints_LineImpl[ItemT](Cmpt_VPoints[ItemT]):
-    '''
-    在线段中，对 :class:`~.Cmpt_VPoints` 的进一步实现
-    '''
-    def copy(self) -> Self:
-        copy_cmpt = super().copy()
-        copy_cmpt.start = self.start.copy()
-        copy_cmpt.end = self.end.copy()
-        # buff 和 path_arc 已经通过 copy.copy(self) 复制
-        return copy_cmpt
-
-    def become(self, other: Cmpt_VPoints_LineImpl) -> Self:
-        super().become(other)
-        self.start = other.start.copy()
-        self.end = other.end.copy()
-        self.buff = other.buff
-        self.path_arc = other.path_arc
-        return self
-
-    def not_changed(self, other) -> bool:
-        return super().not_changed(other)
-
-    def put_start_and_end_on(self, start: Vect, end: Vect) -> Self:
-        curr_start, curr_end = self.get_start_and_end()
-        if np.isclose(curr_start, curr_end).all():
-            # Handle null lines more gracefully
-            self.update_points_by_attrs(start, end, buff=0, path_arc=self.path_arc)
-            return self
-        return self.put_start_and_end_on(start, end)
-
-    def update_points_by_attrs(
-        self,
-        start: np.ndarray | None = None,
-        end: np.ndarray | None = None,
-        buff: float | None = None,
-        path_arc: float | None = None
-    ) -> Self:
-        if start is None:
-            start = self.start
-            assert start is not None
-        else:
-            self.start = start
-
-        if end is None:
-            end = self.end
-            assert end is not None
-        else:
-            self.end = end
-
-        if buff is None:
-            buff = self.buff
-            assert buff is not None
-        else:
-            self.buff = buff
-
-        if path_arc is None:
-            path_arc = self.path_arc
-            assert path_arc is not None
-        else:
-            self.path_arc = path_arc
-
-        builder = PathBuilder(start_point=start)
-        builder.arc_to(end, path_arc)
-        self.set(builder.get())
-
-        # Apply buffer
-        if buff > 0:
-            alpha = min(buff / self.arc_length, 0.5)
-            self.pointwise_become_partial(self, alpha, 1 - alpha)
-        return self
-
-    def set_buff(self, buff: float) -> Self:
-        self.update_points_by_attrs(buff=buff)
-        return self
-
-    def set_path_arc(self, path_arc: float) -> Self:
-        self.update_points_by_attrs(path_arc=path_arc)
-        return self
-
-    def set_start_and_end(self, start: SupportsPointify, end: SupportsPointify) -> Self:
-        start, end = self.pointify_start_and_end(start, end)
-        self.update_points_by_attrs(start=start, end=end)
-        return self
-
-    @staticmethod
-    def pointify_start_and_end(start: SupportsPointify, end: SupportsPointify) -> tuple[np.ndarray, np.ndarray]:
-        # If either start or end are Mobjects, this
-        # gives their centers
-        rough_start = Cmpt_VPoints_LineImpl.pointify(start)
-        rough_end = Cmpt_VPoints_LineImpl.pointify(end)
-        vect = normalize(rough_end - rough_start)
-        # Now that we know the direction between them,
-        # we can find the appropriate boundary point from
-        # start and end, if they're mobjects
-        return (
-            Cmpt_VPoints_LineImpl.pointify(start, vect),
-            Cmpt_VPoints_LineImpl.pointify(end, -vect)
-        )
-
-    @staticmethod
-    def pointify(
-        item_or_data_or_point: SupportsPointify,
-        direction: Vect | None = None
-    ) -> np.ndarray:
-        """
-        Take an argument passed into Line (or subclass) and turn
-        it into a 3d point.
-        """
-        if isinstance(item_or_data_or_point, Points):
-            cmpt = item_or_data_or_point.points
-
-            if direction is None:
-                return cmpt.box.center
-            else:
-                return cmpt.box.get_continuous(direction)
-        else:
-            point = item_or_data_or_point
-            result = np.zeros(3)
-            result[:len(point)] = point
-            return result
-
-    @property
-    def vector(self) -> np.ndarray:
-        return self.get_end() - self.get_start()
-
-    @property
-    def unit_vector(self) -> np.ndarray:
-        return normalize(self.vector)
-
-    @property
-    def angle(self) -> float:
-        return angle_of_vector(self.vector)
-
-    def get_projection(self, point: Vect) -> np.ndarray:
-        """
-        Return projection of a point onto the line
-        """
-        unit_vect = self.unit_vector
-        start = self.get_start()
-        return start + np.dot(point - start, unit_vect) * unit_vect
-
-    def get_slope(self) -> float:
-        return np.tan(self.angle)
-
-    def set_angle(self, angle: float, about_point: Vect | None = None) -> Self:
-        if about_point is None:
-            about_point = self.get_start()
-        self.rotate(
-            angle - self.angle,
-            about_point=about_point,
-        )
-        return self
-
-    def set_length(self, length: float, **kwargs):
-        self.scale(length / self.length, **kwargs)
-        return self
-
-    @property
-    def length(self) -> float:
-        return get_norm(self.vector)
-
-    @property
-    def arc_length(self) -> float:
-        arc_len = get_norm(self.vector)
-        if self.path_arc > 0:
-            arc_len *= self.path_arc / (2 * math.sin(self.path_arc / 2))
-        return arc_len
-
-
-class Line(VItem):
-    '''
-    线段
-
-    传入 ``start``, ``end`` 为线段起点终点
-
-    - ``buff``: 线段两端的空余量，默认为 ``0``
-    - ``path_arc``: 表示线段的弯曲角度
-    '''
-    points = CmptInfo(Cmpt_VPoints_LineImpl[Self])
-
-    def __init__(
-        self,
-        start: Vect | Points = LEFT,
-        end: Vect | Points = RIGHT,
-        *,
-        buff: float = 0,
-        path_arc: float = 0,
-        **kwargs
-    ) -> None:
-        super().__init__(**kwargs)
-
-        start, end = self.points.pointify_start_and_end(start, end)
-        self.points.update_points_by_attrs(start, end, buff, path_arc)
-
-
-# TODO: DashedLine
-
-
-class TangentLine(Line):
-    '''
-    切线
-
-    - 传入 ``vitem`` 表示需要做切线的物件，``alpha`` 表示切点在 ``vitem`` 上的比例
-    - ``length``: 切线长度
-    - ``d_alpha``: 精细程度，越小越精细（默认 ``1e-6``）
-    '''
-    def __init__(
-        self,
-        vitem: VItem,
-        alpha: float,
-        length: float = 1,
-        *,
-        d_alpha: float = 1e-6,
-        **kwargs
-    ) -> None:
-        a1 = clip(alpha - d_alpha, 0, 1)
-        a2 = clip(alpha + d_alpha, 0, 1)
-        super().__init__(vitem.points.pfp(a1), vitem.points.pfp(a2), **kwargs)
-        self.points.scale(length / self.points.length)
-
-
-class Elbow(VItem):
-    '''
-    折线（一般用作直角符号）
-
-    - width 表示宽度
-    - angle 表示角度
-    '''
-    def __init__(
-        self,
-        width: float = 0.2,
-        angle: float = 0,
-        **kwargs
-    ) -> None:
-        super().__init__(**kwargs)
-        self.points.set_as_corners([UP, UP + RIGHT, RIGHT])
-        self.points.set_width(width, about_point=ORIGIN)
-        self.points.rotate(angle, about_point=ORIGIN)
-
-
-# TODO: CubicBezier
+from __future__ import annotations
+
+import math
+from typing import Self
+
+import numpy as np
+
+from janim.components.component import CmptInfo
+from janim.components.vpoints import Cmpt_VPoints
+from janim.constants import LEFT, ORIGIN, RIGHT, UP
+from janim.items.points import Points
+from janim.items.vitem import VItem
+from janim.typing import Vect
+from janim.utils.bezier import PathBuilder
+from janim.utils.simple_functions import clip
+from janim.utils.space_ops import angle_of_vector, get_norm, normalize
+
+type SupportsPointify = Vect | Points
+
+
+class Cmpt_VPoints_LineImpl[ItemT](Cmpt_VPoints[ItemT]):
+    '''
+    在线段中，对 :class:`~.Cmpt_VPoints` 的进一步实现
+    '''
+    def copy(self) -> Self:
+        copy_cmpt = super().copy()
+        copy_cmpt.start = self.start.copy()
+        copy_cmpt.end = self.end.copy()
+        # buff 和 path_arc 已经通过 copy.copy(self) 复制
+        return copy_cmpt
+
+    def become(self, other: Cmpt_VPoints_LineImpl) -> Self:
+        super().become(other)
+        self.start = other.start.copy()
+        self.end = other.end.copy()
+        self.buff = other.buff
+        self.path_arc = other.path_arc
+        return self
+
+    def not_changed(self, other) -> bool:
+        return super().not_changed(other)
+
+    def put_start_and_end_on(self, start: Vect, end: Vect) -> Self:
+        curr_start, curr_end = self.get_start_and_end()
+        if np.isclose(curr_start, curr_end).all():
+            # Handle null lines more gracefully
+            self.update_points_by_attrs(start, end, buff=0, path_arc=self.path_arc)
+            return self
+        return self.put_start_and_end_on(start, end)
+
+    def update_points_by_attrs(
+        self,
+        start: np.ndarray | None = None,
+        end: np.ndarray | None = None,
+        buff: float | None = None,
+        path_arc: float | None = None
+    ) -> Self:
+        if start is None:
+            start = self.start
+            assert start is not None
+        else:
+            self.start = start
+
+        if end is None:
+            end = self.end
+            assert end is not None
+        else:
+            self.end = end
+
+        if buff is None:
+            buff = self.buff
+            assert buff is not None
+        else:
+            self.buff = buff
+
+        if path_arc is None:
+            path_arc = self.path_arc
+            assert path_arc is not None
+        else:
+            self.path_arc = path_arc
+
+        builder = PathBuilder(start_point=start)
+        builder.arc_to(end, path_arc)
+        self.set(builder.get())
+
+        # Apply buffer
+        if buff > 0:
+            alpha = min(buff / self.arc_length, 0.5)
+            self.pointwise_become_partial(self, alpha, 1 - alpha)
+        return self
+
+    def set_buff(self, buff: float) -> Self:
+        self.update_points_by_attrs(buff=buff)
+        return self
+
+    def set_path_arc(self, path_arc: float) -> Self:
+        self.update_points_by_attrs(path_arc=path_arc)
+        return self
+
+    def set_start_and_end(self, start: SupportsPointify, end: SupportsPointify) -> Self:
+        start, end = self.pointify_start_and_end(start, end)
+        self.update_points_by_attrs(start=start, end=end)
+        return self
+
+    @staticmethod
+    def pointify_start_and_end(start: SupportsPointify, end: SupportsPointify) -> tuple[np.ndarray, np.ndarray]:
+        # If either start or end are Mobjects, this
+        # gives their centers
+        rough_start = Cmpt_VPoints_LineImpl.pointify(start)
+        rough_end = Cmpt_VPoints_LineImpl.pointify(end)
+        vect = normalize(rough_end - rough_start)
+        # Now that we know the direction between them,
+        # we can find the appropriate boundary point from
+        # start and end, if they're items
+        return (
+            Cmpt_VPoints_LineImpl.pointify(start, vect),
+            Cmpt_VPoints_LineImpl.pointify(end, -vect)
+        )
+
+    @staticmethod
+    def pointify(
+        item_or_data_or_point: SupportsPointify,
+        direction: Vect | None = None
+    ) -> np.ndarray:
+        """
+        Take an argument passed into Line (or subclass) and turn
+        it into a 3d point.
+        """
+        if isinstance(item_or_data_or_point, Points):
+            cmpt = item_or_data_or_point.points
+
+            if direction is None:
+                return cmpt.box.center
+            else:
+                return cmpt.box.get_continuous(direction)
+        else:
+            point = item_or_data_or_point
+            result = np.zeros(3)
+            result[:len(point)] = point
+            return result
+
+    @property
+    def vector(self) -> np.ndarray:
+        return self.get_end() - self.get_start()
+
+    @property
+    def unit_vector(self) -> np.ndarray:
+        return normalize(self.vector)
+
+    @property
+    def angle(self) -> float:
+        return angle_of_vector(self.vector)
+
+    def get_projection(self, point: Vect) -> np.ndarray:
+        """
+        Return projection of a point onto the line
+        """
+        unit_vect = self.unit_vector
+        start = self.get_start()
+        return start + np.dot(point - start, unit_vect) * unit_vect
+
+    def get_slope(self) -> float:
+        return np.tan(self.angle)
+
+    def set_angle(self, angle: float, about_point: Vect | None = None) -> Self:
+        if about_point is None:
+            about_point = self.get_start()
+        self.rotate(
+            angle - self.angle,
+            about_point=about_point,
+        )
+        return self
+
+    def set_length(self, length: float, **kwargs):
+        self.scale(length / self.length, **kwargs)
+        return self
+
+    @property
+    def length(self) -> float:
+        return get_norm(self.vector)
+
+    @property
+    def arc_length(self) -> float:
+        arc_len = get_norm(self.vector)
+        if self.path_arc > 0:
+            arc_len *= self.path_arc / (2 * math.sin(self.path_arc / 2))
+        return arc_len
+
+
+class Line(VItem):
+    '''
+    线段
+
+    传入 ``start``, ``end`` 为线段起点终点
+
+    - ``buff``: 线段两端的空余量，默认为 ``0``
+    - ``path_arc``: 表示线段的弯曲角度
+    '''
+    points = CmptInfo(Cmpt_VPoints_LineImpl[Self])
+
+    def __init__(
+        self,
+        start: Vect | Points = LEFT,
+        end: Vect | Points = RIGHT,
+        *,
+        buff: float = 0,
+        path_arc: float = 0,
+        **kwargs
+    ) -> None:
+        super().__init__(**kwargs)
+
+        start, end = self.points.pointify_start_and_end(start, end)
+        self.points.update_points_by_attrs(start, end, buff, path_arc)
+
+
+# TODO: DashedLine
+
+
+class TangentLine(Line):
+    '''
+    切线
+
+    - 传入 ``vitem`` 表示需要做切线的物件，``alpha`` 表示切点在 ``vitem`` 上的比例
+    - ``length``: 切线长度
+    - ``d_alpha``: 精细程度，越小越精细（默认 ``1e-6``）
+    '''
+    def __init__(
+        self,
+        vitem: VItem,
+        alpha: float,
+        length: float = 1,
+        *,
+        d_alpha: float = 1e-6,
+        **kwargs
+    ) -> None:
+        a1 = clip(alpha - d_alpha, 0, 1)
+        a2 = clip(alpha + d_alpha, 0, 1)
+        super().__init__(vitem.points.pfp(a1), vitem.points.pfp(a2), **kwargs)
+        self.points.scale(length / self.points.length)
+
+
+class Elbow(VItem):
+    '''
+    折线（一般用作直角符号）
+
+    - width 表示宽度
+    - angle 表示角度
+    '''
+    def __init__(
+        self,
+        width: float = 0.2,
+        angle: float = 0,
+        **kwargs
+    ) -> None:
+        super().__init__(**kwargs)
+        self.points.set_as_corners([UP, UP + RIGHT, RIGHT])
+        self.points.set_width(width, about_point=ORIGIN)
+        self.points.rotate(angle, about_point=ORIGIN)
+
+
+# TODO: CubicBezier
```

### Comparing `janim-1.0.4/janim/items/geometry/polygon.py` & `janim-1.1.0/janim/items/geometry/polygon.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-
-from typing import Iterable, Self, overload
-
-import numpy as np
-
-from janim.constants import DL, DR, PI, RIGHT, UL, UR
-from janim.items.geometry.arc import ArcBetweenPoints
-from janim.items.vitem import VItem
-from janim.typing import Vect, VectArray
-from janim.utils.bezier import PathBuilder
-from janim.utils.iterables import adjacent_n_tuples
-from janim.utils.space_ops import (angle_between_vectors, compass_directions,
-                                   cross2d, get_norm, normalize, rotate_vector)
-
-
-class Polygon(VItem):
-    '''
-    多边形
-
-    传入顶点列表 ``verts`` 进行表示
-    '''
-    def __init__(
-        self,
-        *verts: VectArray,
-        close_path: bool = True,
-        **kwargs
-    ):
-        self.vertices = verts
-        super().__init__(**kwargs)
-        self.points.set_as_corners(
-            [*verts, verts[0]]
-            if close_path
-            else verts
-        )
-
-    def get_vertices(self) -> list[np.ndarray]:
-        return self.points.get()[:-1:2]
-
-    def round_corners(self, radius: float | None = None) -> Self:
-        verts = self.get_vertices()
-        min_edge_length = min(
-            get_norm(v1 - v2)
-            for v1, v2 in zip(verts, verts[1:])
-            if not np.isclose(v1, v2).all()
-        )
-        if radius is None:
-            radius = 0.25 * min_edge_length
-        else:
-            radius = min(radius, 0.5 * min_edge_length)
-        vertices = self.get_vertices()
-        arcs: list[ArcBetweenPoints] = []
-
-        for v1, v2, v3 in adjacent_n_tuples(vertices, 3):
-            vect1 = normalize(v2 - v1)
-            vect2 = normalize(v3 - v2)
-            angle = angle_between_vectors(vect1, vect2)
-            # Distance between vertex and start of the arc
-            cut_off_length = radius * np.tan(angle / 2)
-            # Negative radius gives concave curves
-            sign = float(np.sign(radius * cross2d(vect1, vect2)))
-            arc = ArcBetweenPoints(
-                v2 - vect1 * cut_off_length,
-                v2 + vect2 * cut_off_length,
-                angle=sign * angle,
-                n_components=2,
-            )
-            arcs.append(arc)
-
-        builder = PathBuilder(start_point=arcs[-1].points.get_end())
-        for arc in arcs:
-            if not np.isclose(builder.end_point, arc.points.get_start()).all():
-                builder.line_to(arc.points.get_start())
-            builder.append(arc.points.get()[1:])
-        self.points.set(builder.get())
-        return self
-
-
-class Polyline(Polygon):
-    '''多边形折线
-
-    与 :class:`Polygon` 的区别是，不会自动将最后一个点与第一个点连接
-    '''
-    def __init__(
-        self,
-        *verts: VectArray,
-        close_path: bool = False,
-        **kwargs
-    ):
-        super().__init__(*verts, close_path=close_path, **kwargs)
-
-
-class RegularPolygon(Polygon):
-    '''正多边形
-
-    传入数字 ``n`` 表示边数
-    '''
-    def __init__(
-        self,
-        n: int = 6,
-        *,
-        start_angle: float | None = None,
-        **kwargs
-    ):
-        if start_angle is None:
-            start_angle = (n % 2) * PI / 2
-        start_vect = rotate_vector(RIGHT, start_angle)
-        vertices = compass_directions(n, start_vect)
-        super().__init__(*vertices, **kwargs)
-
-
-class Triangle(RegularPolygon):
-    '''
-    正三角形
-    '''
-    def __init__(self, **kwargs):
-        super().__init__(n=3, **kwargs)
-
-
-class Rect(Polygon):
-    '''矩形
-
-    - 可以使用 ``Rect(4, 2)`` 的传入宽高的方式进行构建
-    - 也可以使用 ``Rect(p1, p2)`` 的传入对角顶点的方式进行构建
-    '''
-    @overload
-    def __init__(self, width: float = 4.0, height: float = 2.0, /, **kwargs) -> None: ...
-    @overload
-    def __init__(self, corner1: Vect, corner2: Vect, /, **kwargs) -> None: ...
-
-    def __init__(self, v1=4.0, v2=2.0, /, **kwargs) -> None:
-        if isinstance(v1, Iterable) and isinstance(v2, Iterable):
-            ul = np.array([min(v1, v2) for v1, v2 in zip(v1, v2)])
-            dr = np.array([max(v1, v2) for v1, v2 in zip(v1, v2)])
-            super().__init__(UR, UL, DL, DR, **kwargs)
-            self.points.set_size(*(dr - ul)[:2])
-            self.points.move_to((dr + ul) / 2)
-
-        else:
-            super().__init__(UR, UL, DL, DR, **kwargs)
-            self.points.set_size(v1, v2)
-
-
-class Square(Rect):
-    '''正方形
-
-    ``side_length`` 表示正方形边长
-    '''
-    def __init__(self, side_length: float = 2.0, **kwargs) -> None:
-        self.side_length = side_length
-        super().__init__(side_length, side_length, **kwargs)
-
-
-class RoundedRect(Rect):
-    '''圆角矩形'''
-    @overload
-    def __init__(self, width: float = 4.0, height: float = 2.0, /, corner_radius: float = 0.5, **kwargs) -> None: ...
-    @overload
-    def __init__(self, corner1: Vect, corner2: Vect, /, corner_radius: float = 0.5, **kwargs) -> None: ...
-
-    def __init__(self, v1=4.0, v2=2.0, /, corner_radius: float = 0.5, **kwargs) -> None:
-        super().__init__(v1, v2, **kwargs)
-        self.round_corners(corner_radius)
+
+from typing import Iterable, Self, overload
+
+import numpy as np
+
+from janim.constants import DL, DR, PI, RIGHT, UL, UR
+from janim.items.geometry.arc import ArcBetweenPoints
+from janim.items.vitem import VItem
+from janim.typing import Vect, VectArray
+from janim.utils.bezier import PathBuilder
+from janim.utils.iterables import adjacent_n_tuples
+from janim.utils.space_ops import (angle_between_vectors, compass_directions,
+                                   cross2d, get_norm, normalize, rotate_vector)
+
+
+class Polygon(VItem):
+    '''
+    多边形
+
+    传入顶点列表 ``verts`` 进行表示
+    '''
+    def __init__(
+        self,
+        *verts: VectArray,
+        close_path: bool = True,
+        **kwargs
+    ):
+        self.vertices = verts
+        super().__init__(**kwargs)
+        self.points.set_as_corners(
+            [*verts, verts[0]]
+            if close_path
+            else verts
+        )
+
+    def get_vertices(self) -> list[np.ndarray]:
+        return self.points.get()[:-1:2]
+
+    def round_corners(self, radius: float | None = None) -> Self:
+        verts = self.get_vertices()
+        min_edge_length = min(
+            get_norm(v1 - v2)
+            for v1, v2 in zip(verts, verts[1:])
+            if not np.isclose(v1, v2).all()
+        )
+        if radius is None:
+            radius = 0.25 * min_edge_length
+        else:
+            radius = min(radius, 0.5 * min_edge_length)
+        vertices = self.get_vertices()
+        arcs: list[ArcBetweenPoints] = []
+
+        for v1, v2, v3 in adjacent_n_tuples(vertices, 3):
+            vect1 = normalize(v2 - v1)
+            vect2 = normalize(v3 - v2)
+            angle = angle_between_vectors(vect1, vect2)
+            # Distance between vertex and start of the arc
+            cut_off_length = radius * np.tan(angle / 2)
+            # Negative radius gives concave curves
+            sign = float(np.sign(radius * cross2d(vect1, vect2)))
+            arc = ArcBetweenPoints(
+                v2 - vect1 * cut_off_length,
+                v2 + vect2 * cut_off_length,
+                angle=sign * angle,
+                n_components=2,
+            )
+            arcs.append(arc)
+
+        builder = PathBuilder(start_point=arcs[-1].points.get_end())
+        for arc in arcs:
+            if not np.isclose(builder.end_point, arc.points.get_start()).all():
+                builder.line_to(arc.points.get_start())
+            builder.append(arc.points.get()[1:])
+        self.points.set(builder.get())
+        return self
+
+
+class Polyline(Polygon):
+    '''多边形折线
+
+    与 :class:`Polygon` 的区别是，不会自动将最后一个点与第一个点连接
+    '''
+    def __init__(
+        self,
+        *verts: VectArray,
+        close_path: bool = False,
+        **kwargs
+    ):
+        super().__init__(*verts, close_path=close_path, **kwargs)
+
+
+class RegularPolygon(Polygon):
+    '''正多边形
+
+    传入数字 ``n`` 表示边数
+    '''
+    def __init__(
+        self,
+        n: int = 6,
+        *,
+        start_angle: float | None = None,
+        **kwargs
+    ):
+        if start_angle is None:
+            start_angle = (n % 2) * PI / 2
+        start_vect = rotate_vector(RIGHT, start_angle)
+        vertices = compass_directions(n, start_vect)
+        super().__init__(*vertices, **kwargs)
+
+
+class Triangle(RegularPolygon):
+    '''
+    正三角形
+    '''
+    def __init__(self, **kwargs):
+        super().__init__(n=3, **kwargs)
+
+
+class Rect(Polygon):
+    '''矩形
+
+    - 可以使用 ``Rect(4, 2)`` 的传入宽高的方式进行构建
+    - 也可以使用 ``Rect(p1, p2)`` 的传入对角顶点的方式进行构建
+    '''
+    @overload
+    def __init__(self, width: float = 4.0, height: float = 2.0, /, **kwargs) -> None: ...
+    @overload
+    def __init__(self, corner1: Vect, corner2: Vect, /, **kwargs) -> None: ...
+
+    def __init__(self, v1=4.0, v2=2.0, /, **kwargs) -> None:
+        if isinstance(v1, Iterable) and isinstance(v2, Iterable):
+            ul = np.array([min(v1, v2) for v1, v2 in zip(v1, v2)])
+            dr = np.array([max(v1, v2) for v1, v2 in zip(v1, v2)])
+            super().__init__(UR, UL, DL, DR, **kwargs)
+            self.points.set_size(*(dr - ul)[:2])
+            self.points.move_to((dr + ul) / 2)
+
+        else:
+            super().__init__(UR, UL, DL, DR, **kwargs)
+            self.points.set_size(v1, v2)
+
+
+class Square(Rect):
+    '''正方形
+
+    ``side_length`` 表示正方形边长
+    '''
+    def __init__(self, side_length: float = 2.0, **kwargs) -> None:
+        self.side_length = side_length
+        super().__init__(side_length, side_length, **kwargs)
+
+
+class RoundedRect(Rect):
+    '''圆角矩形'''
+    @overload
+    def __init__(self, width: float = 4.0, height: float = 2.0, /, corner_radius: float = 0.5, **kwargs) -> None: ...
+    @overload
+    def __init__(self, corner1: Vect, corner2: Vect, /, corner_radius: float = 0.5, **kwargs) -> None: ...
+
+    def __init__(self, v1=4.0, v2=2.0, /, corner_radius: float = 0.5, **kwargs) -> None:
+        super().__init__(v1, v2, **kwargs)
+        self.round_corners(corner_radius)
```

### Comparing `janim-1.0.4/janim/items/image_item.py` & `janim-1.1.0/janim/items/image_item.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-from __future__ import annotations
-
-import math
-
-import moderngl as mgl
-import numpy as np
-
-from janim.components.component import CmptInfo
-from janim.components.image import Cmpt_Image
-from janim.components.rgbas import Cmpt_Rgbas
-from janim.constants import DL, DR, OUT, UL, UR
-from janim.items.points import Points
-from janim.render.impl import ImageItemRenderer
-from janim.render.texture import get_img_from_file
-from janim.utils.config import Config
-from janim.utils.data import AlignedData
-from janim.utils.simple_functions import clip
-from janim.utils.space_ops import cross, det, get_norm, z_to_vector
-
-
-class ImageItem(Points):
-    '''
-    图像物件
-
-    会读取给定的文件路径的图像
-    '''
-
-    renderer_cls = ImageItemRenderer
-
-    image = CmptInfo(Cmpt_Image)
-    color = CmptInfo(Cmpt_Rgbas)
-
-    def __init__(
-        self,
-        file_path: str,
-        *,
-        height: float = None,
-        min_mag_filter: tuple[int, int] = (mgl.LINEAR_MIPMAP_LINEAR, mgl.LINEAR),
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.min_mag_filter = min_mag_filter
-
-        self.points.set([UL, DL, UR, DR])
-
-        img = get_img_from_file(file_path)
-        self.image.set(img, min_mag_filter)
-
-        if height is None:
-            self.points.set_size(
-                img.width * Config.get.pixel_to_frame_ratio,
-                img.height * Config.get.pixel_to_frame_ratio
-            )
-        else:
-            self.points.set_size(
-                height * img.width / img.height,
-                height
-            )
-
-    def get_orig(self) -> np.ndarray:
-        '''图像的左上角'''
-        return self.points.get()[0]
-
-    def get_horizontal_vect(self) -> np.ndarray:
-        '''
-        从图像的左上角指向右上角的向量
-        '''
-        points = self.points.get()
-        return points[2] - points[0]
-
-    def get_horizontal_dist(self) -> float:
-        '''
-        :meth:`get_horizontal_vect` 的长度
-        '''
-        return get_norm(self.get_horizontal_vect())
-
-    def get_vertical_vect(self) -> np.ndarray:
-        '''
-        从图像的左上角指向左下角的向量
-        '''
-        points = self.points.get()
-        return points[1] - points[0]
-
-    def get_vertical_dist(self) -> float:
-        '''
-        :meth:`get_vertical_vect` 的长度
-        '''
-        return get_norm(self.get_vertical_vect())
-
-    def pixel_to_rgba(self, x: int, y: int) -> np.ndarray:
-        '''
-        根据像素坐标得到颜色
-        '''
-        img = self.image.get()
-        width, height = img.size
-        return np.array(
-            img.getpixel((
-                clip(x, 0, width - 1),
-                clip(y, 0, height - 1)
-            ))
-        ) / 255
-
-    def point_to_rgba(self, point: np.ndarray, clamp_to_edge: bool = False) -> np.ndarray:
-        '''
-        通过空间坐标获得对应的像素颜色
-        '''
-        hor = self.get_horizontal_vect()
-        ver = self.get_vertical_vect()
-        vert = point - self.get_orig()
-        normal = cross(hor, ver)
-
-        if not np.isclose(normal, OUT).all():
-            hor, ver, vert = np.dot((hor, ver, vert), z_to_vector(normal))
-
-        u = det(vert, ver) / det(hor, ver)
-        v = det(vert, hor) / det(ver, hor)
-        width, height = self.image.get().size
-        x = math.floor(u * width)
-        y = math.floor(v * height)
-
-        if not clamp_to_edge:
-            if x < 0 or x >= width or y < 0 or y >= height:
-                return np.zeros(4)
-
-        return self.pixel_to_rgba(x, y)
-
-    def pixel_to_point(self, x: float, y: float) -> np.ndarray:
-        '''
-        通过像素坐标获得对应的空间坐标，可以传入浮点值
-
-        - 例如 ``.pixel_to_point(0, 0)`` 会返回原点位置（图片的左上角）
-        - 例如 ``.pixel_to_point(6, 11)`` 会返回 ``(6, 11)`` 像素的左上角
-        - 例如 ``.pixel_to_point(6.5, 11.5)`` 会返回 ``(6, 11)`` 像素的中心
-        '''
-        hor = self.get_horizontal_vect()
-        ver = self.get_vertical_vect()
-        orig = self.get_orig()
-        width, height = self.image.get().size
-
-        return orig + hor * x / width + ver * y / height
-
-    @classmethod
-    def align_for_interpolate(
-        cls,
-        item1: ImageItem,
-        item2: ImageItem,
-    ) -> AlignedData[ImageItem]:
-        aligned = super().align_for_interpolate(item1, item2)
-
-        for data in (aligned.data1, aligned.data2):
-            points_count = data.points.count()
-            data.color.resize(points_count)
-
-        return aligned
-
-
-class PixelImageItem(ImageItem):
-    '''
-    图像物件
-
-    与 :class:`ImageItem` 基本一致，只是在图像被放大显示时不进行平滑插值处理，使得像素清晰
-    '''
-    def __init__(
-        self,
-        file_path: str,
-        *,
-        height: float = None,
-        min_mag_filter: tuple[int, int] = (mgl.LINEAR_MIPMAP_LINEAR, mgl.NEAREST),
-        **kwargs
-    ):
-        super().__init__(file_path, height=height, min_mag_filter=min_mag_filter, **kwargs)
+from __future__ import annotations
+
+import math
+
+import moderngl as mgl
+import numpy as np
+
+from janim.components.component import CmptInfo
+from janim.components.image import Cmpt_Image
+from janim.components.rgbas import Cmpt_Rgbas
+from janim.constants import DL, DR, OUT, UL, UR
+from janim.items.points import Points
+from janim.render.impl import ImageItemRenderer
+from janim.render.texture import get_img_from_file
+from janim.utils.config import Config
+from janim.utils.data import AlignedData
+from janim.utils.simple_functions import clip
+from janim.utils.space_ops import cross, det, get_norm, z_to_vector
+
+
+class ImageItem(Points):
+    '''
+    图像物件
+
+    会读取给定的文件路径的图像
+    '''
+
+    renderer_cls = ImageItemRenderer
+
+    image = CmptInfo(Cmpt_Image)
+    color = CmptInfo(Cmpt_Rgbas)
+
+    def __init__(
+        self,
+        file_path: str,
+        *,
+        height: float = None,
+        min_mag_filter: tuple[int, int] = (mgl.LINEAR_MIPMAP_LINEAR, mgl.LINEAR),
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+        self.min_mag_filter = min_mag_filter
+
+        self.points.set([UL, DL, UR, DR])
+
+        img = get_img_from_file(file_path)
+        self.image.set(img, min_mag_filter)
+
+        if height is None:
+            self.points.set_size(
+                img.width * Config.get.pixel_to_frame_ratio,
+                img.height * Config.get.pixel_to_frame_ratio
+            )
+        else:
+            self.points.set_size(
+                height * img.width / img.height,
+                height
+            )
+
+    def get_orig(self) -> np.ndarray:
+        '''图像的左上角'''
+        return self.points.get()[0]
+
+    def get_horizontal_vect(self) -> np.ndarray:
+        '''
+        从图像的左上角指向右上角的向量
+        '''
+        points = self.points.get()
+        return points[2] - points[0]
+
+    def get_horizontal_dist(self) -> float:
+        '''
+        :meth:`get_horizontal_vect` 的长度
+        '''
+        return get_norm(self.get_horizontal_vect())
+
+    def get_vertical_vect(self) -> np.ndarray:
+        '''
+        从图像的左上角指向左下角的向量
+        '''
+        points = self.points.get()
+        return points[1] - points[0]
+
+    def get_vertical_dist(self) -> float:
+        '''
+        :meth:`get_vertical_vect` 的长度
+        '''
+        return get_norm(self.get_vertical_vect())
+
+    def pixel_to_rgba(self, x: int, y: int) -> np.ndarray:
+        '''
+        根据像素坐标得到颜色
+        '''
+        img = self.image.get()
+        width, height = img.size
+        return np.array(
+            img.getpixel((
+                clip(x, 0, width - 1),
+                clip(y, 0, height - 1)
+            ))
+        ) / 255
+
+    def point_to_rgba(self, point: np.ndarray, clamp_to_edge: bool = False) -> np.ndarray:
+        '''
+        通过空间坐标获得对应的像素颜色
+        '''
+        hor = self.get_horizontal_vect()
+        ver = self.get_vertical_vect()
+        vert = point - self.get_orig()
+        normal = cross(hor, ver)
+
+        if not np.isclose(normal, OUT).all():
+            hor, ver, vert = np.dot((hor, ver, vert), z_to_vector(normal))
+
+        u = det(vert, ver) / det(hor, ver)
+        v = det(vert, hor) / det(ver, hor)
+        width, height = self.image.get().size
+        x = math.floor(u * width)
+        y = math.floor(v * height)
+
+        if not clamp_to_edge:
+            if x < 0 or x >= width or y < 0 or y >= height:
+                return np.zeros(4)
+
+        return self.pixel_to_rgba(x, y)
+
+    def pixel_to_point(self, x: float, y: float) -> np.ndarray:
+        '''
+        通过像素坐标获得对应的空间坐标，可以传入浮点值
+
+        - 例如 ``.pixel_to_point(0, 0)`` 会返回原点位置（图片的左上角）
+        - 例如 ``.pixel_to_point(6, 11)`` 会返回 ``(6, 11)`` 像素的左上角
+        - 例如 ``.pixel_to_point(6.5, 11.5)`` 会返回 ``(6, 11)`` 像素的中心
+        '''
+        hor = self.get_horizontal_vect()
+        ver = self.get_vertical_vect()
+        orig = self.get_orig()
+        width, height = self.image.get().size
+
+        return orig + hor * x / width + ver * y / height
+
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: ImageItem,
+        item2: ImageItem,
+    ) -> AlignedData[ImageItem]:
+        aligned = super().align_for_interpolate(item1, item2)
+
+        for data in (aligned.data1, aligned.data2):
+            points_count = data.points.count()
+            data.color.resize(points_count)
+
+        return aligned
+
+
+class PixelImageItem(ImageItem):
+    '''
+    图像物件
+
+    与 :class:`ImageItem` 基本一致，只是在图像被放大显示时不进行平滑插值处理，使得像素清晰
+    '''
+    def __init__(
+        self,
+        file_path: str,
+        *,
+        height: float = None,
+        min_mag_filter: tuple[int, int] = (mgl.LINEAR_MIPMAP_LINEAR, mgl.NEAREST),
+        **kwargs
+    ):
+        super().__init__(file_path, height=height, min_mag_filter=min_mag_filter, **kwargs)
```

### Comparing `janim-1.0.4/janim/items/item.py` & `janim-1.1.0/janim/items/item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,583 +1,585 @@
-from __future__ import annotations
-
-import copy
-import inspect
-import itertools as it
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, Self, overload
-
-from janim.components.component import CmptInfo, Component, _CmptGroup
-from janim.components.depth import Cmpt_Depth
-from janim.exception import AsTypeError
-from janim.items.relation import Relation
-from janim.logger import log
-from janim.render.base import Renderer
-from janim.typing import SupportsApartAlpha, SupportsInterpolate
-from janim.utils.data import AlignedData
-from janim.utils.iterables import resize_preserving_order
-from janim.utils.paths import PathFunc, straight_path
-
-if TYPE_CHECKING:
-    from janim.items.points import Group
-
-type DynamicItem = Callable[[float], Item]
-
-CLS_CMPTINFO_NAME = '__cls_cmptinfo'
-CLS_STYLES_NAME = '__cls_styles'
-ALL_STYLES_NAME = '__all_styles'
-
-
-class _ItemMeta(type):
-    '''
-    作为 metaclass 记录定义在类中的所有 CmptInfo
-    '''
-    def __new__(cls: type, name: str, bases: tuple[type, ...], attrdict: dict):
-        # 记录所有定义在类中的 CmptInfo
-        cls_components: dict[str, Component] = {
-            key: val
-            for key, val in attrdict.items()
-            if isinstance(val, CmptInfo)
-        }
-        attrdict[CLS_CMPTINFO_NAME] = cls_components
-
-        # 记录 set_style 的参数
-        set_style_func = attrdict.get('set_style', None)
-        if set_style_func is not None and callable(set_style_func):
-            sig = inspect.signature(set_style_func)
-            styles_name: list[str] = [
-                param.name
-                for param in list(sig.parameters.values())[1:]
-                if param.kind not in (param.POSITIONAL_ONLY, param.VAR_POSITIONAL, param.VAR_KEYWORD)
-            ]
-            attrdict[CLS_STYLES_NAME] = styles_name
-
-            all_styles = list(it.chain(
-                styles_name,
-                *[
-                    getattr(base, CLS_STYLES_NAME)
-                    for base in bases
-                    if hasattr(base, CLS_STYLES_NAME)
-                ]
-            ))
-            attrdict[ALL_STYLES_NAME] = all_styles
-
-        return super().__new__(cls, name, bases, attrdict)
-
-
-class Item(Relation['Item'], metaclass=_ItemMeta):
-    renderer_cls = Renderer
-    '''
-    覆盖该值以在子类中使用特定的渲染器
-    '''
-
-    global_renderer: Renderer | None = None
-    '''
-    共用的渲染器，用于 ``is_temporary=True`` 的物件
-    '''
-
-    depth = CmptInfo(Cmpt_Depth[Self], 0)
-
-    def __init__(
-        self,
-        *args,
-        children: list[Item] | None = None,
-        **kwargs
-    ):
-        super().__init__(*args)
-
-        self.stored: bool = False
-        self.stored_parents: list[Item] | None = None
-        self.stored_children: list[Item] | None = None
-
-        # 如果 is_temporary 为 True，则不会另外创建渲染器，而是使用共用的渲染器
-        self.is_temporary: bool = False
-
-        from janim.anims.timeline import Timeline
-        self.timeline = Timeline.get_context(raise_exc=False)
-
-        self._init_components()
-
-        self._astype: type[Item] | None = None
-        self._astype_mock_cmpt: dict[str, Component] = {}
-
-        self.renderer: Renderer | None = None
-
-        if children is not None:
-            self.add(*children)
-        self.digest_styles(**kwargs)
-
-    @dataclass
-    class _CmptInitData:
-        info: CmptInfo[CmptInfo]
-        decl_cls: type[Item]
-
-    def _init_components(self) -> None:
-        '''
-        创建出 CmptInfo 对应的 Component，
-        并以同名存于对象中，起到在名称上覆盖类中的 CmptInfo 的效果
-
-        因为 CmptInfo 的 __get__ 标注的返回类型是对应的 Component，
-        所以以上做法没有影响基于类型标注的代码补全
-        '''
-        type CmptKey = str
-
-        datas: dict[CmptKey, Item._CmptInitData] = {}
-
-        for cls in reversed(self.__class__.mro()):
-            for key, info in cls.__dict__.get(CLS_CMPTINFO_NAME, {}).items():
-                info: CmptInfo
-                if key in datas:
-                    datas[key].info = info
-                else:  # key not in datas
-                    datas[key] = self._CmptInitData(info, cls)
-
-        self.components: dict[str, Component] = {}
-
-        for key, data in datas.items():
-            obj = data.info.create()
-            obj.init_bind(Component.BindInfo(data.decl_cls, self, key))
-
-            self.__dict__[key] = self.components[key] = obj
-
-    def set_component(self, key: str, cmpt: Component) -> None:
-        setattr(self, key, cmpt)
-        self.components[key] = cmpt
-
-    def broadcast_refresh_of_component(
-        self,
-        cmpt: Component,
-        func: Callable | str,
-        *,
-        recurse_up=False,
-        recurse_down=False,
-    ) -> Self:
-        '''
-        为 :meth:`~.Component.mark_refresh()`
-        进行 ``recurse_up/down`` 的处理
-        '''
-        if not recurse_up and not recurse_down:
-            return
-
-        def mark(items: list[Item]):
-            for item in items:
-                if isinstance(item, cmpt.bind.decl_cls):
-                    # 一般情况
-                    item_cmpt: Component = getattr(item, cmpt.bind.key)
-                    item_cmpt.mark_refresh(func)
-
-                else:
-                    # astype 情况
-                    mock_cmpt = item._astype_mock_cmpt.get(cmpt.bind.key, None)
-                    if mock_cmpt is not None:
-                        mock_cmpt.mark_refresh(func)
-
-        if recurse_up:
-            mark(self.ancestors())
-
-        if recurse_down:
-            mark(self.descendants())
-
-    def digest_styles(self, **styles):
-        '''
-        设置物件以及子物件的样式
-        '''
-        flags = dict.fromkeys(styles.keys(), False)
-        for item in self.walk_self_and_descendants():
-            available_styles = item.get_available_styles()
-            apply_styles = {
-                key: style
-                for key, style in styles.items()
-                if key in available_styles
-            }
-            for key in apply_styles:
-                flags[key] = True
-            item.set_style(**apply_styles)
-
-        for key, flag in flags.items():
-            if not flag:
-                log.warning(f'传入参数 "{key}" 没有匹配任何的样式设置，且没有被任何地方使用')
-
-    @classmethod
-    def get_available_styles(cls) -> list[str]:
-        return getattr(cls, ALL_STYLES_NAME)
-
-    def set_style(
-        self,
-        depth: float | None = None,
-        **kwargs
-    ) -> Self:
-        '''
-        设置物件自身的样式，不影响子物件
-        '''
-        if depth is not None:
-            self.depth.set(depth)
-        return self
-
-    def do(self, func: Callable[[Self], Any]) -> Self:
-        '''
-        使用 ``func`` 对物件进行操作，并返回 ``self`` 以方便链式调用
-        '''
-        func(self)
-        return self
-
-    def is_null(self) -> bool:
-        return False
-
-    @property
-    def anim(self) -> Self:
-        '''
-        例如：
-
-        .. code-block:: python
-
-            self.play(
-                item.anim.points.scale(2).r.color.set('green')
-            )
-
-        该例子会创建将 ``item`` 缩放 2 倍并且设置为绿色的补间动画
-
-        并且可以向动画传入参数：
-
-        .. code-block:: python
-
-            self.play(
-                item.anim(duration=2, rate_func=linear)
-                .points.scale(2).r.color.set('green')
-            )
-        '''
-        from janim.anims.transform import MethodTransformArgsBuilder
-        return MethodTransformArgsBuilder(self)
-
-    # 使得 .anim() 后仍有代码提示
-    @overload
-    def __call__(self, **kwargs) -> Self: ...
-
-    @overload
-    def __getitem__(self, value: int) -> Item: ...
-    @overload
-    def __getitem__(self, value: slice) -> Group: ...
-
-    def __getitem__(self, value):
-        if isinstance(value, slice):
-            from janim.items.points import Group
-            return Group(*self.children[value])
-        return self.children[value]
-
-    def __iter__(self):
-        return iter(self.children)
-
-    def __len__(self) -> int:
-        return len(self.children)
-
-    def __mul__(self, other: int) -> Group[Self]:
-        assert isinstance(other, int)
-        return self.replicate(other)
-
-    def replicate(self, n: int) -> Group[Self]:
-        '''
-        复制 n 个自身，并作为一个 :class:`Group` 返回
-
-        可以将 ``item * n`` 作为该方法的简写
-        '''
-        from janim.items.points import Group
-        return Group(
-            *(self.copy() for i in range(n))
-        )
-
-    # region astype
-
-    def astype[T](self, cls: type[T]) -> T:
-        '''
-        使得可以调用当前物件中没有的组件
-
-        例：
-
-        .. code-block:: python
-
-            group = Group(
-                Rect()
-                Circle()
-            )
-
-        在这个例子中，并不能 ``group.color.set(BLUE)`` 来设置子物件中的颜色，
-        但是可以使用 ``group.astype(VItem).color.set(BLUE)`` 来做到
-
-        也可以使用简写 ``group(VItem).color.set(BLUE)``
-        '''
-        if not isinstance(cls, type) or not issubclass(cls, Item):
-            # TODO: i18n
-            raise AsTypeError(f'{cls.__name__} 不是以 Item 为基类，无法作为 astype 的参数')
-
-        self._astype = cls
-        return self
-
-    @overload
-    def __call__[T](self, cls: type[T]) -> T: ...
-
-    def __call__[T](self, cls: type[T]) -> T:
-        '''
-        等效于调用 ``astype``
-        '''
-        return self.astype(cls)
-
-    def __getattr__(self, name: str):
-        if name == '__setstate__':
-            raise AttributeError()
-
-        cmpt_info = None if self._astype is None else getattr(self._astype, name, None)
-        if not isinstance(cmpt_info, CmptInfo):
-            super().__getattribute__(name)  # raise error
-
-        # 找到 cmpt_info 是在哪个类中被定义的
-        decl_cls: type[Item] | None = None
-        for sup in self._astype.mro():
-            if name in sup.__dict__.get(CLS_CMPTINFO_NAME, {}):
-                decl_cls = sup
-
-        assert decl_cls is not None
-
-        # 如果 self 本身就是 decl_cls 的实例
-        # 那么自身肯定有名称为 name 的组件，对于这种情况实际上完全没必要 astype
-        # 为了灵活性，这里将这个已有的组件返回
-        if isinstance(self, decl_cls):
-            return getattr(self, name)
-
-        cmpt = self._astype_mock_cmpt.get(name, None)
-
-        # 如果 astype 需求的组件已经被创建过，并且新类型不是旧类型的子类，那么直接返回
-        if cmpt is not None and (not issubclass(cmpt_info.cls, cmpt.__class__) or cmpt_info.cls is cmpt.__class__):
-            return cmpt
-
-        # astype 需求的组件还没创建，那么创建并记录
-        cmpt = cmpt_info.create()
-        cmpt.init_bind(Component.BindInfo(decl_cls, self, name))
-
-        self._astype_mock_cmpt[name] = cmpt
-        return cmpt
-
-    # endregion
-
-    # region data
-
-    def get_parents(self):
-        return self.stored_parents if self.stored else self.parents
-
-    def get_children(self):
-        return self.stored_children if self.stored else self.children
-
-    def not_changed(self, other: Self) -> bool:
-        if self.get_children() != other.get_children():
-            return False
-        for key, cmpt in self.components.items():
-            if not cmpt.not_changed(other.components[key]):
-                return False
-        return True
-
-    def current(self, *, as_time: float | None = None, skip_dynamic=False) -> Self:
-        '''
-        当前物件
-
-        - 如果此时在回放和 Updater 中，则返回对应时间的历史物件
-        - 在其余情况下，包括该物件没有历史记录的情况，则返回物件自身
-        '''
-        return self.timeline.item_current(self, as_time=as_time, skip_dynamic=skip_dynamic)
-
-    def copy(self, *, root_only=False) -> Self:
-        '''
-        复制物件
-        '''
-        copy_item = copy.copy(self)
-
-        copy_item.reset_refresh()
-
-        copy_item.parents = []
-        copy_item.children = []
-        if root_only:
-            copy_item.stored = True
-            copy_item.stored_parents = self.get_parents().copy()
-            copy_item.stored_children = self.get_children().copy()
-        else:
-            copy_item.add(*[item.copy() for item in self.children])
-            copy_item.parents_changed()
-
-        new_cmpts = {}
-        for key, cmpt in self.components.items():
-            if isinstance(cmpt, _CmptGroup):
-                # 因为现在的 Python 版本中，dict 取键值保留原序
-                # 所以 new_cmpts 肯定有 _CmptGroup 所需要的
-                cmpt_copy = cmpt.copy(new_cmpts=new_cmpts)
-            else:
-                cmpt_copy = cmpt.copy()
-
-            if cmpt.bind is not None:
-                cmpt_copy.init_bind(Component.BindInfo(cmpt.bind.decl_cls,
-                                                       copy_item,
-                                                       key))
-
-            new_cmpts[key] = cmpt_copy
-            setattr(copy_item, key, cmpt_copy)
-
-        copy_item.components = new_cmpts
-        copy_item._astype_mock_cmpt = {}
-
-        return copy_item
-
-    # TODO: optimize
-    def _current_family(self, *, up: bool) -> list[Item]:   # use DFS
-        lst = self.stored_parents if up else self.stored_children
-        res = []
-
-        for sub_obj in lst:
-            current = sub_obj.current()
-            if current not in res:
-                res.append(current)
-            res.extend(filter(
-                lambda obj: obj not in res,
-                current._current_family(up=up)
-                if current.stored
-                else (current.ancestors() if up else current.descendants())
-            ))
-
-        return res
-
-    def become(self, other: Item) -> Self:
-        '''
-        将该物件的数据设置为与传入的物件相同（以复制的方式，不是引用）
-        '''
-        # self.parents 不变
-
-        children = self.children.copy()
-        self.clear_children()
-        for old, new in it.zip_longest(children, other.children):
-            if new is None:
-                break
-            if old is None or type(old) is not type(new):
-                self.add(new.copy())
-            else:
-                self.add(old.become(new))
-
-        for key in self.components.keys() | other.components.keys():
-            self.components[key].become(other.components[key])
-
-        from janim.anims.timeline import Timeline
-        timeline = Timeline.get_context(raise_exc=False)
-        if timeline is not None and timeline.is_displaying(self):
-            timeline.show(self)
-
-        return self
-
-    def store(self) -> Self:
-        return self.copy(root_only=True)
-
-    def restore(self, other: Item) -> Self:
-        self.parents = other.parents.copy()
-        self.parents_changed()
-        self.children = other.children.copy()
-        self.children_changed()
-
-        for key in self.components.keys() & other.components.keys():
-            self.components[key].become(other.components[key])
-
-        return self
-
-    @classmethod
-    def align_for_interpolate(
-        cls,
-        item1: Item,
-        item2: Item
-    ) -> AlignedData[Self]:
-        '''
-        进行数据对齐，以便插值
-        '''
-        aligned = AlignedData(item1.store(),
-                              item1.store(),
-                              item2.store())
-
-        # align components
-        for key, cmpt1 in item1.components.items():
-            cmpt2 = item2.components.get(key, None)
-
-            if isinstance(cmpt1, _CmptGroup) and isinstance(cmpt2, _CmptGroup):
-                cmpt_aligned = cmpt1.align(cmpt1, cmpt2, aligned)
-
-            elif cmpt2 is None or not isinstance(cmpt1, SupportsInterpolate):
-                cmpt_aligned = AlignedData(cmpt1, cmpt1, cmpt1)
-            else:
-                cmpt_aligned = cmpt1.align_for_interpolate(cmpt1, cmpt2)
-
-            aligned.data1.set_component(key, cmpt_aligned.data1)
-            aligned.data2.set_component(key, cmpt_aligned.data2)
-            aligned.union.set_component(key, cmpt_aligned.union)
-
-        # align children
-        max_len = max(len(item1.get_children()), len(item2.get_children()))
-        aligned.data1.stored_children = resize_preserving_order(item1.get_children(), max_len)
-        aligned.data2.stored_children = resize_preserving_order(item2.get_children(), max_len)
-
-        return aligned
-
-    def interpolate(
-        self,
-        item1: Item,
-        item2: Item,
-        alpha: float,
-        *,
-        path_func: PathFunc = straight_path,
-    ) -> None:
-        '''
-        进行插值（仅对该物件进行，不包含后代物件）
-        '''
-        for key, cmpt in self.components.items():
-            cmpt1 = item1.components[key]
-            cmpt2 = item2.components[key]
-
-            if not isinstance(cmpt, SupportsInterpolate):
-                continue
-
-            cmpt.interpolate(cmpt1, cmpt2, alpha, path_func=path_func)
-
-    def apart_alpha(self, n: int) -> None:
-        for cmpt in self.components.values():
-            if isinstance(cmpt, SupportsApartAlpha):
-                cmpt.apart_alpha(n)
-
-    @classmethod
-    def get_global_renderer(cls) -> None:
-        if cls.global_renderer is None:
-            cls.global_renderer = cls.renderer_cls()
-        return cls.global_renderer
-
-    def create_renderer(self) -> None:
-        if self.is_temporary:
-            self.renderer = self.get_global_renderer()
-        else:
-            self.renderer = self.renderer_cls()
-
-    def render(self) -> None:
-        if self.renderer is None:
-            self.create_renderer()
-
-        if not self.renderer.initialized:
-            self.renderer.init()
-            self.renderer.initialized = True
-        self.renderer.render(self)
-
-    # endregion
-
-    # region timeline
-
-    def show(self, **kwargs) -> Self:
-        '''
-        显示物件
-        '''
-        self.timeline.show(self, **kwargs)
-        return self
-
-    def hide(self, **kwargs) -> Self:
-        '''
-        隐藏物件
-        '''
-        self.timeline.hide(self, **kwargs)
-        return self
-
-    # endregion
+from __future__ import annotations
+
+import copy
+import inspect
+import itertools as it
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Callable, Self, overload
+
+from janim.components.component import CmptInfo, Component, _CmptGroup
+from janim.components.depth import Cmpt_Depth
+from janim.exception import AsTypeError
+from janim.items.relation import Relation
+from janim.logger import log
+from janim.render.base import Renderer
+from janim.typing import SupportsApartAlpha, SupportsInterpolate
+from janim.utils.data import AlignedData
+from janim.utils.iterables import resize_preserving_order
+from janim.utils.paths import PathFunc, straight_path
+
+if TYPE_CHECKING:
+    from janim.items.points import Group
+
+type DynamicItem = Callable[[float], Item]
+
+CLS_CMPTINFO_NAME = '__cls_cmptinfo'
+CLS_STYLES_NAME = '__cls_styles'
+ALL_STYLES_NAME = '__all_styles'
+
+
+class _ItemMeta(type):
+    '''
+    作为 metaclass 记录定义在类中的所有 CmptInfo
+    '''
+    def __new__(cls: type, name: str, bases: tuple[type, ...], attrdict: dict):
+        # 记录所有定义在类中的 CmptInfo
+        cls_components: dict[str, Component] = {
+            key: val
+            for key, val in attrdict.items()
+            if isinstance(val, CmptInfo)
+        }
+        attrdict[CLS_CMPTINFO_NAME] = cls_components
+
+        # 记录 set_style 的参数
+        set_style_func = attrdict.get('set_style', None)
+        if set_style_func is not None and callable(set_style_func):
+            sig = inspect.signature(set_style_func)
+            styles_name: list[str] = [
+                param.name
+                for param in list(sig.parameters.values())[1:]
+                if param.kind not in (param.POSITIONAL_ONLY, param.VAR_POSITIONAL, param.VAR_KEYWORD)
+            ]
+            attrdict[CLS_STYLES_NAME] = styles_name
+
+            all_styles = list(it.chain(
+                styles_name,
+                *[
+                    getattr(base, CLS_STYLES_NAME)
+                    for base in bases
+                    if hasattr(base, CLS_STYLES_NAME)
+                ]
+            ))
+            attrdict[ALL_STYLES_NAME] = all_styles
+
+        return super().__new__(cls, name, bases, attrdict)
+
+
+class Item(Relation['Item'], metaclass=_ItemMeta):
+    renderer_cls = Renderer
+    '''
+    覆盖该值以在子类中使用特定的渲染器
+    '''
+
+    global_renderer: Renderer | None = None
+    '''
+    共用的渲染器，用于 ``is_temporary=True`` 的物件
+    '''
+
+    depth = CmptInfo(Cmpt_Depth[Self], 0)
+
+    def __init__(
+        self,
+        *args,
+        children: list[Item] | None = None,
+        **kwargs
+    ):
+        super().__init__(*args)
+
+        self.stored: bool = False
+        self.stored_parents: list[Item] | None = None
+        self.stored_children: list[Item] | None = None
+
+        # 如果 is_temporary 为 True，则不会另外创建渲染器，而是使用共用的渲染器
+        self.is_temporary: bool = False
+
+        from janim.anims.timeline import Timeline
+        self.timeline = Timeline.get_context(raise_exc=False)
+
+        self._init_components()
+
+        self._astype: type[Item] | None = None
+        self._astype_mock_cmpt: dict[str, Component] = {}
+
+        self.renderer: Renderer | None = None
+
+        if children is not None:
+            self.add(*children)
+        self.digest_styles(**kwargs)
+
+    @dataclass
+    class _CmptInitData:
+        info: CmptInfo[CmptInfo]
+        decl_cls: type[Item]
+
+    def _init_components(self) -> None:
+        '''
+        创建出 CmptInfo 对应的 Component，
+        并以同名存于对象中，起到在名称上覆盖类中的 CmptInfo 的效果
+
+        因为 CmptInfo 的 __get__ 标注的返回类型是对应的 Component，
+        所以以上做法没有影响基于类型标注的代码补全
+        '''
+        type CmptKey = str
+
+        datas: dict[CmptKey, Item._CmptInitData] = {}
+
+        for cls in reversed(self.__class__.mro()):
+            for key, info in cls.__dict__.get(CLS_CMPTINFO_NAME, {}).items():
+                info: CmptInfo
+                if key in datas:
+                    datas[key].info = info
+                else:  # key not in datas
+                    datas[key] = self._CmptInitData(info, cls)
+
+        self.components: dict[str, Component] = {}
+
+        for key, data in datas.items():
+            obj = data.info.create()
+            obj.init_bind(Component.BindInfo(data.decl_cls, self, key))
+
+            self.__dict__[key] = self.components[key] = obj
+
+    def set_component(self, key: str, cmpt: Component) -> None:
+        setattr(self, key, cmpt)
+        self.components[key] = cmpt
+
+    def broadcast_refresh_of_component(
+        self,
+        cmpt: Component,
+        func: Callable | str,
+        *,
+        recurse_up=False,
+        recurse_down=False,
+    ) -> Self:
+        '''
+        为 :meth:`~.Component.mark_refresh()`
+        进行 ``recurse_up/down`` 的处理
+        '''
+        if not recurse_up and not recurse_down:
+            return
+
+        def mark(items: list[Item]):
+            for item in items:
+                if isinstance(item, cmpt.bind.decl_cls):
+                    # 一般情况
+                    item_cmpt: Component = getattr(item, cmpt.bind.key)
+                    item_cmpt.mark_refresh(func)
+
+                else:
+                    # astype 情况
+                    mock_cmpt = item._astype_mock_cmpt.get(cmpt.bind.key, None)
+                    if mock_cmpt is not None:
+                        mock_cmpt.mark_refresh(func)
+
+        if recurse_up:
+            mark(self.ancestors())
+
+        if recurse_down:
+            mark(self.descendants())
+
+    def digest_styles(self, **styles):
+        '''
+        设置物件以及子物件的样式
+        '''
+        flags = dict.fromkeys(styles.keys(), False)
+        for item in self.walk_self_and_descendants():
+            available_styles = item.get_available_styles()
+            apply_styles = {
+                key: style
+                for key, style in styles.items()
+                if key in available_styles
+            }
+            for key in apply_styles:
+                flags[key] = True
+            item.set_style(**apply_styles)
+
+        for key, flag in flags.items():
+            if not flag:
+                log.warning(f'传入参数 "{key}" 没有匹配任何的样式设置，且没有被任何地方使用')
+
+    @classmethod
+    def get_available_styles(cls) -> list[str]:
+        return getattr(cls, ALL_STYLES_NAME)
+
+    def set_style(
+        self,
+        depth: float | None = None,
+        **kwargs
+    ) -> Self:
+        '''
+        设置物件自身的样式，不影响子物件
+        '''
+        if depth is not None:
+            self.depth.set(depth)
+        return self
+
+    def do(self, func: Callable[[Self], Any]) -> Self:
+        '''
+        使用 ``func`` 对物件进行操作，并返回 ``self`` 以方便链式调用
+        '''
+        func(self)
+        return self
+
+    def is_null(self) -> bool:
+        return False
+
+    @property
+    def anim(self) -> Self:
+        '''
+        例如：
+
+        .. code-block:: python
+
+            self.play(
+                item.anim.points.scale(2).r.color.set('green')
+            )
+
+        该例子会创建将 ``item`` 缩放 2 倍并且设置为绿色的补间动画
+
+        并且可以向动画传入参数：
+
+        .. code-block:: python
+
+            self.play(
+                item.anim(duration=2, rate_func=linear)
+                .points.scale(2).r.color.set('green')
+            )
+
+        ``.r`` 表示从组件回到物件，这样就可以调用其它组件的功能
+        '''
+        from janim.anims.transform import MethodTransformArgsBuilder
+        return MethodTransformArgsBuilder(self)
+
+    # 使得 .anim() 后仍有代码提示
+    @overload
+    def __call__(self, **kwargs) -> Self: ...
+
+    @overload
+    def __getitem__(self, value: int) -> Item: ...
+    @overload
+    def __getitem__(self, value: slice) -> Group: ...
+
+    def __getitem__(self, value):
+        if isinstance(value, slice):
+            from janim.items.points import Group
+            return Group(*self.children[value])
+        return self.children[value]
+
+    def __iter__(self):
+        return iter(self.children)
+
+    def __len__(self) -> int:
+        return len(self.children)
+
+    def __mul__(self, other: int) -> Group[Self]:
+        assert isinstance(other, int)
+        return self.replicate(other)
+
+    def replicate(self, n: int) -> Group[Self]:
+        '''
+        复制 n 个自身，并作为一个 :class:`Group` 返回
+
+        可以将 ``item * n`` 作为该方法的简写
+        '''
+        from janim.items.points import Group
+        return Group(
+            *(self.copy() for i in range(n))
+        )
+
+    # region astype
+
+    def astype[T](self, cls: type[T]) -> T:
+        '''
+        使得可以调用当前物件中没有的组件
+
+        例：
+
+        .. code-block:: python
+
+            group = Group(
+                Rect()
+                Circle()
+            )
+
+        在这个例子中，并不能 ``group.color.set(BLUE)`` 来设置子物件中的颜色，
+        但是可以使用 ``group.astype(VItem).color.set(BLUE)`` 来做到
+
+        也可以使用简写 ``group(VItem).color.set(BLUE)``
+        '''
+        if not isinstance(cls, type) or not issubclass(cls, Item):
+            # TODO: i18n
+            raise AsTypeError(f'{cls.__name__} 不是以 Item 为基类，无法作为 astype 的参数')
+
+        self._astype = cls
+        return self
+
+    @overload
+    def __call__[T](self, cls: type[T]) -> T: ...
+
+    def __call__[T](self, cls: type[T]) -> T:
+        '''
+        等效于调用 ``astype``
+        '''
+        return self.astype(cls)
+
+    def __getattr__(self, name: str):
+        if name == '__setstate__':
+            raise AttributeError()
+
+        cmpt_info = None if self._astype is None else getattr(self._astype, name, None)
+        if not isinstance(cmpt_info, CmptInfo):
+            super().__getattribute__(name)  # raise error
+
+        # 找到 cmpt_info 是在哪个类中被定义的
+        decl_cls: type[Item] | None = None
+        for sup in self._astype.mro():
+            if name in sup.__dict__.get(CLS_CMPTINFO_NAME, {}):
+                decl_cls = sup
+
+        assert decl_cls is not None
+
+        # 如果 self 本身就是 decl_cls 的实例
+        # 那么自身肯定有名称为 name 的组件，对于这种情况实际上完全没必要 astype
+        # 为了灵活性，这里将这个已有的组件返回
+        if isinstance(self, decl_cls):
+            return getattr(self, name)
+
+        cmpt = self._astype_mock_cmpt.get(name, None)
+
+        # 如果 astype 需求的组件已经被创建过，并且新类型不是旧类型的子类，那么直接返回
+        if cmpt is not None and (not issubclass(cmpt_info.cls, cmpt.__class__) or cmpt_info.cls is cmpt.__class__):
+            return cmpt
+
+        # astype 需求的组件还没创建，那么创建并记录
+        cmpt = cmpt_info.create()
+        cmpt.init_bind(Component.BindInfo(decl_cls, self, name))
+
+        self._astype_mock_cmpt[name] = cmpt
+        return cmpt
+
+    # endregion
+
+    # region data
+
+    def get_parents(self):
+        return self.stored_parents if self.stored else self.parents
+
+    def get_children(self):
+        return self.stored_children if self.stored else self.children
+
+    def not_changed(self, other: Self) -> bool:
+        if self.get_children() != other.get_children():
+            return False
+        for key, cmpt in self.components.items():
+            if not cmpt.not_changed(other.components[key]):
+                return False
+        return True
+
+    def current(self, *, as_time: float | None = None, skip_dynamic=False) -> Self:
+        '''
+        当前物件
+
+        - 如果此时在回放和 Updater 中，则返回对应时间的历史物件
+        - 在其余情况下，包括该物件没有历史记录的情况，则返回物件自身
+        '''
+        return self.timeline.item_current(self, as_time=as_time, skip_dynamic=skip_dynamic)
+
+    def copy(self, *, root_only=False) -> Self:
+        '''
+        复制物件
+        '''
+        copy_item = copy.copy(self)
+
+        copy_item.reset_refresh()
+
+        copy_item.parents = []
+        copy_item.children = []
+        if root_only:
+            copy_item.stored = True
+            copy_item.stored_parents = self.get_parents().copy()
+            copy_item.stored_children = self.get_children().copy()
+        else:
+            copy_item.add(*[item.copy() for item in self.children])
+            copy_item.parents_changed()
+
+        new_cmpts = {}
+        for key, cmpt in self.components.items():
+            if isinstance(cmpt, _CmptGroup):
+                # 因为现在的 Python 版本中，dict 取键值保留原序
+                # 所以 new_cmpts 肯定有 _CmptGroup 所需要的
+                cmpt_copy = cmpt.copy(new_cmpts=new_cmpts)
+            else:
+                cmpt_copy = cmpt.copy()
+
+            if cmpt.bind is not None:
+                cmpt_copy.init_bind(Component.BindInfo(cmpt.bind.decl_cls,
+                                                       copy_item,
+                                                       key))
+
+            new_cmpts[key] = cmpt_copy
+            setattr(copy_item, key, cmpt_copy)
+
+        copy_item.components = new_cmpts
+        copy_item._astype_mock_cmpt = {}
+
+        return copy_item
+
+    # TODO: optimize
+    def _current_family(self, *, up: bool) -> list[Item]:   # use DFS
+        lst = self.stored_parents if up else self.stored_children
+        res = []
+
+        for sub_obj in lst:
+            current = sub_obj.current()
+            if current not in res:
+                res.append(current)
+            res.extend(filter(
+                lambda obj: obj not in res,
+                current._current_family(up=up)
+                if current.stored
+                else (current.ancestors() if up else current.descendants())
+            ))
+
+        return res
+
+    def become(self, other: Item) -> Self:
+        '''
+        将该物件的数据设置为与传入的物件相同（以复制的方式，不是引用）
+        '''
+        # self.parents 不变
+
+        children = self.children.copy()
+        self.clear_children()
+        for old, new in it.zip_longest(children, other.children):
+            if new is None:
+                break
+            if old is None or type(old) is not type(new):
+                self.add(new.copy())
+            else:
+                self.add(old.become(new))
+
+        for key in self.components.keys() | other.components.keys():
+            self.components[key].become(other.components[key])
+
+        from janim.anims.timeline import Timeline
+        timeline = Timeline.get_context(raise_exc=False)
+        if timeline is not None and timeline.is_displaying(self):
+            timeline.show(self)
+
+        return self
+
+    def store(self) -> Self:
+        return self.copy(root_only=True)
+
+    def restore(self, other: Item) -> Self:
+        self.parents = other.parents.copy()
+        self.parents_changed()
+        self.children = other.children.copy()
+        self.children_changed()
+
+        for key in self.components.keys() & other.components.keys():
+            self.components[key].become(other.components[key])
+
+        return self
+
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: Item,
+        item2: Item
+    ) -> AlignedData[Self]:
+        '''
+        进行数据对齐，以便插值
+        '''
+        aligned = AlignedData(item1.store(),
+                              item1.store(),
+                              item2.store())
+
+        # align components
+        for key, cmpt1 in item1.components.items():
+            cmpt2 = item2.components.get(key, None)
+
+            if isinstance(cmpt1, _CmptGroup) and isinstance(cmpt2, _CmptGroup):
+                cmpt_aligned = cmpt1.align(cmpt1, cmpt2, aligned)
+
+            elif cmpt2 is None or not isinstance(cmpt1, SupportsInterpolate):
+                cmpt_aligned = AlignedData(cmpt1, cmpt1, cmpt1)
+            else:
+                cmpt_aligned = cmpt1.align_for_interpolate(cmpt1, cmpt2)
+
+            aligned.data1.set_component(key, cmpt_aligned.data1)
+            aligned.data2.set_component(key, cmpt_aligned.data2)
+            aligned.union.set_component(key, cmpt_aligned.union)
+
+        # align children
+        max_len = max(len(item1.get_children()), len(item2.get_children()))
+        aligned.data1.stored_children = resize_preserving_order(item1.get_children(), max_len)
+        aligned.data2.stored_children = resize_preserving_order(item2.get_children(), max_len)
+
+        return aligned
+
+    def interpolate(
+        self,
+        item1: Item,
+        item2: Item,
+        alpha: float,
+        *,
+        path_func: PathFunc = straight_path,
+    ) -> None:
+        '''
+        进行插值（仅对该物件进行，不包含后代物件）
+        '''
+        for key, cmpt in self.components.items():
+            cmpt1 = item1.components[key]
+            cmpt2 = item2.components[key]
+
+            if not isinstance(cmpt, SupportsInterpolate):
+                continue
+
+            cmpt.interpolate(cmpt1, cmpt2, alpha, path_func=path_func)
+
+    def apart_alpha(self, n: int) -> None:
+        for cmpt in self.components.values():
+            if isinstance(cmpt, SupportsApartAlpha):
+                cmpt.apart_alpha(n)
+
+    @classmethod
+    def get_global_renderer(cls) -> None:
+        if cls.global_renderer is None:
+            cls.global_renderer = cls.renderer_cls()
+        return cls.global_renderer
+
+    def create_renderer(self) -> None:
+        if self.is_temporary:
+            self.renderer = self.get_global_renderer()
+        else:
+            self.renderer = self.renderer_cls()
+
+    def render(self) -> None:
+        if self.renderer is None:
+            self.create_renderer()
+
+        if not self.renderer.initialized:
+            self.renderer.init()
+            self.renderer.initialized = True
+        self.renderer.render(self)
+
+    # endregion
+
+    # region timeline
+
+    def show(self, **kwargs) -> Self:
+        '''
+        显示物件
+        '''
+        self.timeline.show(self, **kwargs)
+        return self
+
+    def hide(self, **kwargs) -> Self:
+        '''
+        隐藏物件
+        '''
+        self.timeline.hide(self, **kwargs)
+        return self
+
+    # endregion
```

### Comparing `janim-1.0.4/janim/items/points.py` & `janim-1.1.0/janim/items/points.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from __future__ import annotations
-
-from typing import Iterable, Self, overload
-
-from janim.components.component import CmptInfo
-from janim.components.points import Cmpt_Points
-from janim.components.radius import Cmpt_Radius
-from janim.components.rgbas import Cmpt_Rgbas, apart_alpha
-from janim.items.item import Item
-from janim.render.impl import DotCloudRenderer
-from janim.typing import ColorArray, JAnimColor, Vect
-from janim.utils.data import AlignedData
-from janim.utils.iterables import (resize_preserving_order,
-                                   resize_preserving_order_indice_groups)
-
-
-class Points(Item):
-    '''
-    点集
-
-    纯数据物件，不参与渲染
-    '''
-    points = CmptInfo(Cmpt_Points[Self])
-
-    def __init__(self, *points: Vect, **kwargs):
-        super().__init__(**kwargs)
-
-        if points:
-            self.points.set(points)
-
-    def is_null(self) -> bool:
-        return not self.points.has()
-
-
-class Group[T](Points):
-    '''
-    将物件组成一组
-    '''
-    def __init__(self, *objs: T, **kwargs):
-        super().__init__(children=objs, **kwargs)
-
-        self.children: list[T]
-
-    @overload
-    def __getitem__(self, value: int) -> T: ...
-    @overload
-    def __getitem__(self, value: slice) -> Group[T]: ...
-
-    def __getitem__(self, value):   # pragma: no cover
-        return super().__getitem__(value)
-
-    def __iter__(self):
-        return iter(self.children)
-
-
-class DotCloud(Points):
-    color = CmptInfo(Cmpt_Rgbas[Self])
-    radius = CmptInfo(Cmpt_Radius[Self], 0.05)
-
-    renderer_cls = DotCloudRenderer
-
-    def __init__(
-        self,
-        *args,
-
-        **kwargs
-    ):
-        super().__init__(*args, **kwargs)
-
-        Cmpt_Points.reverse.connect(self.points, lambda: self.radius.reverse())
-
-        self.points.resize_func = resize_preserving_order
-
-    def set_style(
-        self,
-        color: JAnimColor | ColorArray | None = None,
-        alpha: float | Iterable[float] | None = None,
-        radius: float | Iterable[float] | None = None,
-        **kwargs
-    ) -> Self:
-        self.color.set(color, alpha, root_only=True)
-        if radius is not None:
-            self.radius.set(radius, root_only=True)
-
-        return super().set_style(**kwargs)
-
-    @classmethod
-    def align_for_interpolate(
-        cls,
-        item1: DotCloud,
-        item2: DotCloud,
-    ) -> AlignedData[DotCloud]:
-        len1 = len(item1.points.get())
-        len2 = len(item2.points.get())
-
-        aligned = super().align_for_interpolate(item1, item2)
-
-        for data in (aligned.data1, aligned.data2):
-            points_count = data.points.count()
-            data.color.resize(points_count)
-            data.radius.resize(points_count)
-
-        if len1 != len2:
-            indice_groups = resize_preserving_order_indice_groups(min(len1, len2), max(len1, len2))
-
-            cmpt_to_fade = aligned.data1.color if len1 < len2 else aligned.data2.color
-            rgbas = cmpt_to_fade.get().copy()
-            for group in indice_groups:
-                rgbas[group, 3] = apart_alpha(rgbas[group[0], 3], len(group))
-            cmpt_to_fade.set_rgbas(rgbas)
-
-        return aligned
+from __future__ import annotations
+
+from typing import Iterable, Self, overload
+
+from janim.components.component import CmptInfo
+from janim.components.points import Cmpt_Points
+from janim.components.radius import Cmpt_Radius
+from janim.components.rgbas import Cmpt_Rgbas, apart_alpha
+from janim.items.item import Item
+from janim.render.impl import DotCloudRenderer
+from janim.typing import ColorArray, JAnimColor, Vect
+from janim.utils.data import AlignedData
+from janim.utils.iterables import (resize_preserving_order,
+                                   resize_preserving_order_indice_groups)
+
+
+class Points(Item):
+    '''
+    点集
+
+    纯数据物件，不参与渲染
+    '''
+    points = CmptInfo(Cmpt_Points[Self])
+
+    def __init__(self, *points: Vect, **kwargs):
+        super().__init__(**kwargs)
+
+        if points:
+            self.points.set(points)
+
+    def is_null(self) -> bool:
+        return not self.points.has()
+
+
+class Group[T](Points):
+    '''
+    将物件组成一组
+    '''
+    def __init__(self, *objs: T, **kwargs):
+        super().__init__(children=objs, **kwargs)
+
+        self.children: list[T]
+
+    @overload
+    def __getitem__(self, value: int) -> T: ...
+    @overload
+    def __getitem__(self, value: slice) -> Group[T]: ...
+
+    def __getitem__(self, value):   # pragma: no cover
+        return super().__getitem__(value)
+
+    def __iter__(self):
+        return iter(self.children)
+
+
+class DotCloud(Points):
+    color = CmptInfo(Cmpt_Rgbas[Self])
+    radius = CmptInfo(Cmpt_Radius[Self], 0.05)
+
+    renderer_cls = DotCloudRenderer
+
+    def __init__(
+        self,
+        *args,
+
+        **kwargs
+    ):
+        super().__init__(*args, **kwargs)
+
+        Cmpt_Points.reverse.connect(self.points, lambda: self.radius.reverse())
+
+        self.points.resize_func = resize_preserving_order
+
+    def set_style(
+        self,
+        color: JAnimColor | ColorArray | None = None,
+        alpha: float | Iterable[float] | None = None,
+        radius: float | Iterable[float] | None = None,
+        **kwargs
+    ) -> Self:
+        self.color.set(color, alpha, root_only=True)
+        if radius is not None:
+            self.radius.set(radius, root_only=True)
+
+        return super().set_style(**kwargs)
+
+    @classmethod
+    def align_for_interpolate(
+        cls,
+        item1: DotCloud,
+        item2: DotCloud,
+    ) -> AlignedData[DotCloud]:
+        len1 = len(item1.points.get())
+        len2 = len(item2.points.get())
+
+        aligned = super().align_for_interpolate(item1, item2)
+
+        for data in (aligned.data1, aligned.data2):
+            points_count = data.points.count()
+            data.color.resize(points_count)
+            data.radius.resize(points_count)
+
+        if len1 != len2:
+            indice_groups = resize_preserving_order_indice_groups(min(len1, len2), max(len1, len2))
+
+            cmpt_to_fade = aligned.data1.color if len1 < len2 else aligned.data2.color
+            rgbas = cmpt_to_fade.get().copy()
+            for group in indice_groups:
+                rgbas[group, 3] = apart_alpha(rgbas[group[0], 3], len(group))
+            cmpt_to_fade.set_rgbas(rgbas)
+
+        return aligned
```

### Comparing `janim-1.0.4/janim/items/relation.py` & `janim-1.1.0/janim/items/relation.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-from __future__ import annotations
-
-import random
-from typing import Callable, Generator, Self
-
-import janim.utils.refresh as refresh
-from janim.utils.signal import Signal
-
-
-class Relation[GRelT: 'Relation'](refresh.Refreshable):
-    '''
-    定义了有向无环图的包含关系以及一些实用操作
-
-    也就是，对于每个对象：
-
-    - ``self.parents`` 存储了与其直接关联的父对象
-    - ``self.children`` 存储了与其直接关联的子对象
-    - 使用 :meth:`add()` 建立对象间的关系
-    - 使用 :meth:`remove()` 取消对象间的关系
-    - :meth:`ancestors()` 表示与其直接关联的祖先对象（包括父对象，以及父对象的父对象，......）
-    - :meth:`descendants()` 表示与其直接关联的后代对象（包括子对象、以及子对象的子对象，......）
-    - 对于 :meth:`ancestors()` 以及 :meth:`descendants()`：
-        - 不包含调用者自身并且返回的列表中没有重复元素
-        - 物件顺序是 DFS 顺序
-    '''
-    def __init__(self):
-        super().__init__()
-
-        self.parents: list[GRelT] = []
-        self.children: list[GRelT] = []
-
-    def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
-        super().mark_refresh(func)
-
-        name = func.__name__ if callable(func) else func
-
-        if recurse_up:
-            for obj in self.ancestors():
-                if hasattr(obj, name):
-                    obj.mark_refresh(name)
-
-        if recurse_down:
-            for obj in self.descendants():
-                if hasattr(obj, name):
-                    obj.mark_refresh(name)
-
-    @Signal
-    def parents_changed(self) -> None:
-        '''
-        信号，在 ``self.parents`` 改变时触发
-        '''
-        Relation.parents_changed.emit(self)
-
-    @Signal
-    def children_changed(self) -> None:
-        '''
-        信号，在 ``self.children`` 改变时触发
-        '''
-        Relation.children_changed.emit(self)
-
-    def add(self, *objs: GRelT, insert=False) -> Self:
-        '''
-        向该对象添加子对象
-
-        如果 ``insert=True`` （默认为 ``False``），那么插入到子物件列表的开头
-        '''
-        for obj in (reversed(objs) if insert else objs):
-            # 理论上这里判断 item not in self.children 就够了，但是防止
-            # 有被私自修改 self.parents 以及 self.children 的可能，所以这里都判断了
-            # Theoretically, checking item not in self.children is enough here, but to prevent
-            # possible modifications to self.parents and self.children, both checks are made here.
-            if obj not in self.children:
-                if insert:
-                    self.children.insert(0, obj)
-                else:
-                    self.children.append(obj)
-            if self not in obj.parents:
-                obj.parents.append(self)
-            obj.parents_changed()
-
-        self.children_changed()
-        return self
-
-    def remove(self, *objs: GRelT) -> Self:
-        '''
-        从该对象移除子对象
-        '''
-        for obj in objs:
-            # 理论上这里判断 `item in self.children` 就够了，原因同 `add`
-            # Theoretically, checking `item in self.children` is enough here, for the same reason as `add`.
-            try:
-                self.children.remove(obj)
-            except ValueError: ...
-            try:
-                obj.parents.remove(self)
-            except ValueError: ...
-            obj.parents_changed()
-
-        self.children_changed()
-        return self
-
-    def shuffle(self) -> Self:
-        random.shuffle(self.children)
-        self.children_changed()
-        return self
-
-    def clear_parents(self) -> Self:
-        for parent in self.parents:
-            parent.remove(self)
-        return self
-
-    def clear_children(self) -> Self:
-        self.remove(*self.children)
-        return self
-
-    def _family(self, *, up: bool) -> list[GRelT]:  # use DFS
-        lst = self.parents if up else self.children
-        res = []
-
-        for sub_obj in lst:
-            if sub_obj not in res:
-                res.append(sub_obj)
-            res.extend(filter(
-                lambda obj: obj not in res,
-                sub_obj._family(up=up)
-            ))
-
-        return res
-
-    @parents_changed.self_refresh_with_recurse(recurse_down=True)
-    @refresh.register
-    def ancestors(self) -> list[GRelT]:
-        '''
-        获得祖先对象列表
-        '''
-        return self._family(up=True)
-
-    @children_changed.self_refresh_with_recurse(recurse_up=True)
-    @refresh.register
-    def descendants(self) -> list[GRelT]:
-        '''
-        获得后代对象列表
-        '''
-        return self._family(up=False)
-
-    @staticmethod
-    def _walk_lst[RelT](base_cls: type[RelT] | None, lst: list[GRelT]) -> Generator[RelT, None, None]:
-        if base_cls is None:
-            yield from lst
-            return
-
-        for obj in lst:
-            if isinstance(obj, base_cls):
-                yield obj
-
-    def _walk_nearest_family[RelT](
-        self: Relation,
-        base_cls: type[RelT],
-        fn_family: Callable[[Relation], list[Relation]],
-    ) -> Generator[RelT, None, None]:
-
-        lst = fn_family(self)[:]
-
-        while lst:
-            obj = lst.pop(0)
-            if isinstance(obj, base_cls):
-                # DFS 结构保证了使用该做法进行剔除的合理性
-                # DFS structure ensures the validity of using this method for removal.
-                for sub_obj in fn_family(obj):
-                    if not lst:
-                        break
-                    if lst[0] is sub_obj:
-                        lst.pop(0)
-                yield obj
-
-    def walk_ancestors[RelT](self, base_cls: type[RelT] = None) -> Generator[RelT, None, None]:
-        '''
-        遍历祖先节点中以 ``base_cls`` （缺省则遍历全部）为基类的对象
-        '''
-        yield from self._walk_lst(base_cls, self.ancestors())
-
-    def walk_descendants[RelT](self, base_cls: type[RelT] = None) -> Generator[RelT, None, None]:
-        '''
-        遍历后代节点中以 ``base_cls`` （缺省则遍历全部）为基类的对象
-        '''
-        yield from self._walk_lst(base_cls, self.descendants())
-
-    def walk_self_and_ancestors(self, root_only=False) -> Generator[GRelT, None, None]:
-        '''
-        遍历自己以及祖先节点
-        '''
-        yield self
-        if not root_only:
-            yield from self.ancestors()
-
-    def walk_self_and_descendants(self, root_only=False) -> Generator[GRelT, None, None]:
-        '''
-        遍历自己以及后代节点
-        '''
-        yield self
-        if not root_only:
-            yield from self.descendants()
-
-    def walk_nearest_ancestors[RelT](self, base_cls: type[RelT]) -> Generator[RelT, None, None]:
-        '''
-        遍历祖先节点中以 ``base_cls`` 为基类的对象，但是排除已经满足条件的对象的祖先对象
-        '''
-        yield from self._walk_nearest_family(base_cls, lambda rel: rel.ancestors())
-
-    def walk_nearest_descendants[RelT](self, base_cls: type[RelT]) -> Generator[RelT, None, None]:
-        '''
-        遍历后代节点中以 ``base_cls`` 为基类的对象，但是排除已经满足条件的对象的后代对象
-        '''
-        yield from self._walk_nearest_family(base_cls, lambda rel: rel.descendants())
+from __future__ import annotations
+
+import random
+from typing import Callable, Generator, Self
+
+import janim.utils.refresh as refresh
+from janim.utils.signal import Signal
+
+
+class Relation[GRelT: 'Relation'](refresh.Refreshable):
+    '''
+    定义了有向无环图的包含关系以及一些实用操作
+
+    也就是，对于每个对象：
+
+    - ``self.parents`` 存储了与其直接关联的父对象
+    - ``self.children`` 存储了与其直接关联的子对象
+    - 使用 :meth:`add()` 建立对象间的关系
+    - 使用 :meth:`remove()` 取消对象间的关系
+    - :meth:`ancestors()` 表示与其直接关联的祖先对象（包括父对象，以及父对象的父对象，......）
+    - :meth:`descendants()` 表示与其直接关联的后代对象（包括子对象、以及子对象的子对象，......）
+    - 对于 :meth:`ancestors()` 以及 :meth:`descendants()`：
+        - 不包含调用者自身并且返回的列表中没有重复元素
+        - 物件顺序是 DFS 顺序
+    '''
+    def __init__(self):
+        super().__init__()
+
+        self.parents: list[GRelT] = []
+        self.children: list[GRelT] = []
+
+    def mark_refresh(self, func: Callable | str, *, recurse_up=False, recurse_down=False) -> Self:
+        super().mark_refresh(func)
+
+        name = func.__name__ if callable(func) else func
+
+        if recurse_up:
+            for obj in self.ancestors():
+                if hasattr(obj, name):
+                    obj.mark_refresh(name)
+
+        if recurse_down:
+            for obj in self.descendants():
+                if hasattr(obj, name):
+                    obj.mark_refresh(name)
+
+    @Signal
+    def parents_changed(self) -> None:
+        '''
+        信号，在 ``self.parents`` 改变时触发
+        '''
+        Relation.parents_changed.emit(self)
+
+    @Signal
+    def children_changed(self) -> None:
+        '''
+        信号，在 ``self.children`` 改变时触发
+        '''
+        Relation.children_changed.emit(self)
+
+    def add(self, *objs: GRelT, insert=False) -> Self:
+        '''
+        向该对象添加子对象
+
+        如果 ``insert=True`` （默认为 ``False``），那么插入到子物件列表的开头
+        '''
+        for obj in (reversed(objs) if insert else objs):
+            # 理论上这里判断 item not in self.children 就够了，但是防止
+            # 有被私自修改 self.parents 以及 self.children 的可能，所以这里都判断了
+            # Theoretically, checking item not in self.children is enough here, but to prevent
+            # possible modifications to self.parents and self.children, both checks are made here.
+            if obj not in self.children:
+                if insert:
+                    self.children.insert(0, obj)
+                else:
+                    self.children.append(obj)
+            if self not in obj.parents:
+                obj.parents.append(self)
+            obj.parents_changed()
+
+        self.children_changed()
+        return self
+
+    def remove(self, *objs: GRelT) -> Self:
+        '''
+        从该对象移除子对象
+        '''
+        for obj in objs:
+            # 理论上这里判断 `item in self.children` 就够了，原因同 `add`
+            # Theoretically, checking `item in self.children` is enough here, for the same reason as `add`.
+            try:
+                self.children.remove(obj)
+            except ValueError: ...
+            try:
+                obj.parents.remove(self)
+            except ValueError: ...
+            obj.parents_changed()
+
+        self.children_changed()
+        return self
+
+    def shuffle(self) -> Self:
+        random.shuffle(self.children)
+        self.children_changed()
+        return self
+
+    def clear_parents(self) -> Self:
+        for parent in self.parents:
+            parent.remove(self)
+        return self
+
+    def clear_children(self) -> Self:
+        self.remove(*self.children)
+        return self
+
+    def _family(self, *, up: bool) -> list[GRelT]:  # use DFS
+        lst = self.parents if up else self.children
+        res = []
+
+        for sub_obj in lst:
+            if sub_obj not in res:
+                res.append(sub_obj)
+            res.extend(filter(
+                lambda obj: obj not in res,
+                sub_obj._family(up=up)
+            ))
+
+        return res
+
+    @parents_changed.self_refresh_with_recurse(recurse_down=True)
+    @refresh.register
+    def ancestors(self) -> list[GRelT]:
+        '''
+        获得祖先对象列表
+        '''
+        return self._family(up=True)
+
+    @children_changed.self_refresh_with_recurse(recurse_up=True)
+    @refresh.register
+    def descendants(self) -> list[GRelT]:
+        '''
+        获得后代对象列表
+        '''
+        return self._family(up=False)
+
+    @staticmethod
+    def _walk_lst[RelT](base_cls: type[RelT] | None, lst: list[GRelT]) -> Generator[RelT, None, None]:
+        if base_cls is None:
+            yield from lst
+            return
+
+        for obj in lst:
+            if isinstance(obj, base_cls):
+                yield obj
+
+    def _walk_nearest_family[RelT](
+        self: Relation,
+        base_cls: type[RelT],
+        fn_family: Callable[[Relation], list[Relation]],
+    ) -> Generator[RelT, None, None]:
+
+        lst = fn_family(self)[:]
+
+        while lst:
+            obj = lst.pop(0)
+            if isinstance(obj, base_cls):
+                # DFS 结构保证了使用该做法进行剔除的合理性
+                # DFS structure ensures the validity of using this method for removal.
+                for sub_obj in fn_family(obj):
+                    if not lst:
+                        break
+                    if lst[0] is sub_obj:
+                        lst.pop(0)
+                yield obj
+
+    def walk_ancestors[RelT](self, base_cls: type[RelT] = None) -> Generator[RelT, None, None]:
+        '''
+        遍历祖先节点中以 ``base_cls`` （缺省则遍历全部）为基类的对象
+        '''
+        yield from self._walk_lst(base_cls, self.ancestors())
+
+    def walk_descendants[RelT](self, base_cls: type[RelT] = None) -> Generator[RelT, None, None]:
+        '''
+        遍历后代节点中以 ``base_cls`` （缺省则遍历全部）为基类的对象
+        '''
+        yield from self._walk_lst(base_cls, self.descendants())
+
+    def walk_self_and_ancestors(self, root_only=False) -> Generator[GRelT, None, None]:
+        '''
+        遍历自己以及祖先节点
+        '''
+        yield self
+        if not root_only:
+            yield from self.ancestors()
+
+    def walk_self_and_descendants(self, root_only=False) -> Generator[GRelT, None, None]:
+        '''
+        遍历自己以及后代节点
+        '''
+        yield self
+        if not root_only:
+            yield from self.descendants()
+
+    def walk_nearest_ancestors[RelT](self, base_cls: type[RelT]) -> Generator[RelT, None, None]:
+        '''
+        遍历祖先节点中以 ``base_cls`` 为基类的对象，但是排除已经满足条件的对象的祖先对象
+        '''
+        yield from self._walk_nearest_family(base_cls, lambda rel: rel.ancestors())
+
+    def walk_nearest_descendants[RelT](self, base_cls: type[RelT]) -> Generator[RelT, None, None]:
+        '''
+        遍历后代节点中以 ``base_cls`` 为基类的对象，但是排除已经满足条件的对象的后代对象
+        '''
+        yield from self._walk_nearest_family(base_cls, lambda rel: rel.descendants())
```

### Comparing `janim-1.0.4/janim/items/shape_matchers.py` & `janim-1.1.0/janim/items/shape_matchers.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from __future__ import annotations
-
-from janim.constants import DOWN, LEFT, RIGHT, SMALL_BUFF, UP, YELLOW
-from janim.items.geometry.line import Line
-from janim.items.geometry.polygon import Rect
-from janim.items.points import Points
-from janim.typing import JAnimColor
-from janim.utils.config import Config
-from janim.utils.data import Align, Margins, MarginsType
-
-
-class SurroundingRect(Rect):
-    def __init__(
-        self,
-        item: Points,
-        *,
-        buff: MarginsType = SMALL_BUFF,
-        color: JAnimColor = YELLOW,
-        width: float | None = None,
-        height: float | None = None,
-        align: Align = Align.Center,
-        **kwargs
-    ):
-        if not isinstance(buff, Margins):
-            buff = Margins(buff)
-        if width is None:
-            width = item.points.box.width + buff.left + buff.right
-        if height is None:
-            height = item.points.box.height + buff.top + buff.bottom
-
-        super().__init__(width, height, color=color, **kwargs)
-
-        if align & Align.Left:
-            x = item.points.box.get_x(LEFT) - buff.left + width / 2
-        elif align & Align.Right:
-            x = item.points.box.get_x(RIGHT) + buff.right - width / 2
-        else:
-            x = item.points.box.get_x() + (buff.right - buff.left) / 2
-
-        if align & Align.Bottom:
-            y = item.points.box.get_y(DOWN) - buff.bottom + height / 2
-        elif align & Align.Top:
-            y = item.points.box.get_y(UP) + buff.top - height / 2
-        else:
-            y = item.points.box.get_y() + (buff.top - buff.bottom) / 2
-
-        self.points.move_to([x, y, 0])
-
-
-class FrameRect(Rect):
-    def __init__(self, **kwargs):
-        super().__init__(Config.get.frame_width, Config.get.frame_height, **kwargs)
-
-
-class Underline(Line):
-    def __init__(self, item: Points, *, buff: float = SMALL_BUFF, **kwargs):
-        super().__init__(LEFT, RIGHT, **kwargs)
-        self.points.set_width(item.points.box.width)
-        self.points.next_to(item, DOWN, buff=buff)
+from __future__ import annotations
+
+from janim.constants import DOWN, LEFT, RIGHT, SMALL_BUFF, UP, YELLOW
+from janim.items.geometry.line import Line
+from janim.items.geometry.polygon import Rect
+from janim.items.points import Points
+from janim.typing import JAnimColor
+from janim.utils.config import Config
+from janim.utils.data import Align, Margins, MarginsType
+
+
+class SurroundingRect(Rect):
+    def __init__(
+        self,
+        item: Points,
+        *,
+        buff: MarginsType = SMALL_BUFF,
+        color: JAnimColor = YELLOW,
+        width: float | None = None,
+        height: float | None = None,
+        align: Align = Align.Center,
+        **kwargs
+    ):
+        if not isinstance(buff, Margins):
+            buff = Margins(buff)
+        if width is None:
+            width = item.points.box.width + buff.left + buff.right
+        if height is None:
+            height = item.points.box.height + buff.top + buff.bottom
+
+        super().__init__(width, height, color=color, **kwargs)
+
+        if align & Align.Left:
+            x = item.points.box.get_x(LEFT) - buff.left + width / 2
+        elif align & Align.Right:
+            x = item.points.box.get_x(RIGHT) + buff.right - width / 2
+        else:
+            x = item.points.box.get_x() + (buff.right - buff.left) / 2
+
+        if align & Align.Bottom:
+            y = item.points.box.get_y(DOWN) - buff.bottom + height / 2
+        elif align & Align.Top:
+            y = item.points.box.get_y(UP) + buff.top - height / 2
+        else:
+            y = item.points.box.get_y() + (buff.top - buff.bottom) / 2
+
+        self.points.move_to([x, y, 0])
+
+
+class FrameRect(Rect):
+    def __init__(self, **kwargs):
+        super().__init__(Config.get.frame_width, Config.get.frame_height, **kwargs)
+
+
+class Underline(Line):
+    def __init__(self, item: Points, *, buff: float = SMALL_BUFF, **kwargs):
+        super().__init__(LEFT, RIGHT, **kwargs)
+        self.points.set_width(item.points.box.width)
+        self.points.next_to(item, DOWN, buff=buff)
```

### Comparing `janim-1.0.4/janim/items/svg/brace.py` & `janim-1.1.0/janim/items/svg/brace.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-
-import math
-import os
-from typing import Self
-
-import numpy as np
-
-from janim.components.component import CmptInfo
-from janim.components.vpoints import Cmpt_VPoints
-from janim.constants import DEFAULT_ITEM_TO_ITEM_BUFF, DOWN, PI, SMALL_BUFF
-from janim.items.points import Points
-from janim.items.svg.svg_item import SVGItem
-from janim.items.svg.typst import Typst
-from janim.items.text.text import Text
-from janim.items.vitem import VItem
-from janim.typing import Vect
-from janim.utils.file_ops import get_janim_dir
-from janim.utils.space_ops import normalize, rotation_about_z
-
-
-class Cmpt_VPoints_BraceImpl[ItemT](Cmpt_VPoints[ItemT], impl=True):
-    '''
-    在 :class:`Brace` 中对 :class:`Cmpt_VPoints` 的进一步实现
-    '''
-    # 复制时，``brace_length`` 随 ``copy.copy(self)`` 而复制，因此不用重写 ``copy`` 方法
-    def match(
-        self,
-        item: Points | None,
-        direction: Vect | None = None,
-        buff: float = SMALL_BUFF,
-        root_only: bool = False
-    ) -> Self:
-        '''
-        将花括号进行伸缩，使得与 ``item`` 在 ``direction`` 方向的宽度匹配
-        '''
-        if direction is None:
-            direction = self.direction if self.has() else DOWN
-
-        self.set(get_brace_orig_points())
-
-        angle = math.atan2(direction[1], direction[0]) + PI / 2
-        rot = np.array(rotation_about_z(-angle))
-
-        if item is None:
-            self.brace_length = self.box.width
-        else:
-            cmpt = item.points
-
-            rot_points = np.dot(
-                cmpt.get() if root_only else cmpt.get_all(),
-                rot.T
-            )   # dot(points, rot.T) == dot(rot, points.T).T
-
-            box = self.BoundingBox(rot_points)
-            self.brace_length = box.width
-
-            self.set_width(box.width, stretch=box.width > self.box.width)
-            self.move_to(box.bottom + DOWN * (buff + self.box.height / 2))
-
-        self.apply_matrix(rot.T)     # rot.T == rot.I
-
-        return self
-
-    @property
-    def tip_point(self) -> np.ndarray:
-        '''得到花括号中间凸出处的坐标'''
-        return self._points.data[get_brace_tip_point_index()]
-
-    @property
-    def brace_left(self) -> np.ndarray:
-        '''得到括号指向方向左边的尖端处的坐标'''
-        return self._points.data[get_brace_left_index()]
-
-    @property
-    def brace_right(self) -> np.ndarray:
-        '''得到括号指向方向右边的尖端处的坐标'''
-        return self._points.data[get_brace_right_index()]
-
-    @property
-    def direction(self) -> np.ndarray:
-        '''得到括号指向的方向'''
-        return normalize(self.tip_point - self.box.center)
-
-    def put_at_tip(
-        self,
-        item: Points,
-        use_next_to: bool = True,
-        buff: float = DEFAULT_ITEM_TO_ITEM_BUFF,
-        **kwargs
-    ) -> Self:
-        '''
-        将物件放置在花括号中间的凸出处
-        '''
-        cmpt = item.points
-
-        if use_next_to:
-            cmpt.next_to(
-                self.tip_point,
-                np.round(self.direction),
-                buff=buff,
-                **kwargs
-            )
-        else:
-            cmpt.move_to(self.tip_point)
-            shift_distance = cmpt.box.width * 0.5 + buff
-            cmpt.shift(self.direction * shift_distance)
-
-    def create_text(self, text: str, buff: float = SMALL_BUFF, use_next_to: bool = True, **kwargs) -> Text:
-        '''创建一个位于花括号中间凸出处的文字'''
-        txt = Text(text, **kwargs)
-        self.put_at_tip(txt, use_next_to=use_next_to, buff=buff)
-        return txt
-
-    def create_typst(self, typst: str, buff: float = SMALL_BUFF, use_next_to: bool = True, **kwargs) -> Typst:
-        '''创建一个位于花括号中间凸出处的 Typst 公式'''
-        typ = Typst(typst, **kwargs)
-        self.put_at_tip(typ, use_next_to=use_next_to, buff=buff)
-        return typ
-
-
-class Brace(VItem):
-    '''
-    花括号物件
-
-    会匹配物件在 ``direction`` 方向的宽度
-    '''
-    points = CmptInfo(Cmpt_VPoints_BraceImpl[Self])
-
-    def __init__(
-        self,
-        item: Points | None = None,
-        direction: np.ndarray = DOWN,
-        buff: float = SMALL_BUFF,
-        stroke_alpha: float = 0,
-        fill_alpha: float = 1,
-        **kwargs
-    ):
-        super().__init__(stroke_alpha=stroke_alpha, fill_alpha=fill_alpha, **kwargs)
-        self.points.match(item, direction, buff)
-
-
-brace_orig_points: np.ndarray | None = None
-brace_tip_point_index: int | None = None
-brace_left_index: int | None = None
-brace_right_index: int | None = None
-
-
-def get_brace_orig_points() -> np.ndarray:
-    global brace_orig_points
-    if brace_orig_points is not None:
-        return brace_orig_points
-
-    svg = SVGItem(os.path.join(get_janim_dir(), 'items', 'svg', 'brace.svg'))
-    points = svg[0].points.get()
-    center = (points.min(axis=0) + points.max(axis=0)) * 0.5
-
-    brace_orig_points = points - center
-    return brace_orig_points
-
-
-def get_brace_tip_point_index() -> int:
-    global brace_tip_point_index
-    if brace_tip_point_index is not None:
-        return brace_tip_point_index
-
-    points = get_brace_orig_points()
-    brace_tip_point_index = points[:, 1].argmin()
-
-    return brace_tip_point_index
-
-
-def get_brace_left_index() -> int:
-    global brace_left_index
-    if brace_left_index is not None:
-        return brace_left_index
-
-    points = get_brace_orig_points()
-    brace_left_index = points[:, 0].argmin()
-
-    return brace_left_index
-
-
-def get_brace_right_index() -> int:
-    global brace_left_index
-    if brace_left_index is not None:
-        return brace_left_index
-
-    points = get_brace_orig_points()
-    brace_left_index = points[:, 0].argmax()
-
-    return brace_left_index
+
+import math
+import os
+from typing import Self
+
+import numpy as np
+
+from janim.components.component import CmptInfo
+from janim.components.vpoints import Cmpt_VPoints
+from janim.constants import DEFAULT_ITEM_TO_ITEM_BUFF, DOWN, PI, SMALL_BUFF
+from janim.items.points import Points
+from janim.items.svg.svg_item import SVGItem
+from janim.items.svg.typst import Typst
+from janim.items.text.text import Text
+from janim.items.vitem import VItem
+from janim.typing import Vect
+from janim.utils.file_ops import get_janim_dir
+from janim.utils.space_ops import normalize, rotation_about_z
+
+
+class Cmpt_VPoints_BraceImpl[ItemT](Cmpt_VPoints[ItemT], impl=True):
+    '''
+    在 :class:`Brace` 中对 :class:`Cmpt_VPoints` 的进一步实现
+    '''
+    # 复制时，``brace_length`` 随 ``copy.copy(self)`` 而复制，因此不用重写 ``copy`` 方法
+    def match(
+        self,
+        item: Points | None,
+        direction: Vect | None = None,
+        buff: float = SMALL_BUFF,
+        root_only: bool = False
+    ) -> Self:
+        '''
+        将花括号进行伸缩，使得与 ``item`` 在 ``direction`` 方向的宽度匹配
+        '''
+        if direction is None:
+            direction = self.direction if self.has() else DOWN
+
+        self.set(get_brace_orig_points())
+
+        angle = math.atan2(direction[1], direction[0]) + PI / 2
+        rot = np.array(rotation_about_z(-angle))
+
+        if item is None:
+            self.brace_length = self.box.width
+        else:
+            cmpt = item.points
+
+            rot_points = np.dot(
+                cmpt.get() if root_only else cmpt.get_all(),
+                rot.T
+            )   # dot(points, rot.T) == dot(rot, points.T).T
+
+            box = self.BoundingBox(rot_points)
+            self.brace_length = box.width
+
+            self.set_width(box.width, stretch=box.width > self.box.width)
+            self.move_to(box.bottom + DOWN * (buff + self.box.height / 2))
+
+        self.apply_matrix(rot.T)     # rot.T == rot.I
+
+        return self
+
+    @property
+    def tip_point(self) -> np.ndarray:
+        '''得到花括号中间凸出处的坐标'''
+        return self._points.data[get_brace_tip_point_index()]
+
+    @property
+    def brace_left(self) -> np.ndarray:
+        '''得到括号指向方向左边的尖端处的坐标'''
+        return self._points.data[get_brace_left_index()]
+
+    @property
+    def brace_right(self) -> np.ndarray:
+        '''得到括号指向方向右边的尖端处的坐标'''
+        return self._points.data[get_brace_right_index()]
+
+    @property
+    def direction(self) -> np.ndarray:
+        '''得到括号指向的方向'''
+        return normalize(self.tip_point - self.box.center)
+
+    def put_at_tip(
+        self,
+        item: Points,
+        use_next_to: bool = True,
+        buff: float = DEFAULT_ITEM_TO_ITEM_BUFF,
+        **kwargs
+    ) -> Self:
+        '''
+        将物件放置在花括号中间的凸出处
+        '''
+        cmpt = item.points
+
+        if use_next_to:
+            cmpt.next_to(
+                self.tip_point,
+                np.round(self.direction),
+                buff=buff,
+                **kwargs
+            )
+        else:
+            cmpt.move_to(self.tip_point)
+            shift_distance = cmpt.box.width * 0.5 + buff
+            cmpt.shift(self.direction * shift_distance)
+
+    def create_text(self, text: str, buff: float = SMALL_BUFF, use_next_to: bool = True, **kwargs) -> Text:
+        '''创建一个位于花括号中间凸出处的文字'''
+        txt = Text(text, **kwargs)
+        self.put_at_tip(txt, use_next_to=use_next_to, buff=buff)
+        return txt
+
+    def create_typst(self, typst: str, buff: float = SMALL_BUFF, use_next_to: bool = True, **kwargs) -> Typst:
+        '''创建一个位于花括号中间凸出处的 Typst 公式'''
+        typ = Typst(typst, **kwargs)
+        self.put_at_tip(typ, use_next_to=use_next_to, buff=buff)
+        return typ
+
+
+class Brace(VItem):
+    '''
+    花括号物件
+
+    会匹配物件在 ``direction`` 方向的宽度
+    '''
+    points = CmptInfo(Cmpt_VPoints_BraceImpl[Self])
+
+    def __init__(
+        self,
+        item: Points | None = None,
+        direction: np.ndarray = DOWN,
+        buff: float = SMALL_BUFF,
+        stroke_alpha: float = 0,
+        fill_alpha: float = 1,
+        **kwargs
+    ):
+        super().__init__(stroke_alpha=stroke_alpha, fill_alpha=fill_alpha, **kwargs)
+        self.points.match(item, direction, buff)
+
+
+brace_orig_points: np.ndarray | None = None
+brace_tip_point_index: int | None = None
+brace_left_index: int | None = None
+brace_right_index: int | None = None
+
+
+def get_brace_orig_points() -> np.ndarray:
+    global brace_orig_points
+    if brace_orig_points is not None:
+        return brace_orig_points
+
+    svg = SVGItem(os.path.join(get_janim_dir(), 'items', 'svg', 'brace.svg'))
+    points = svg[0].points.get()
+    center = (points.min(axis=0) + points.max(axis=0)) * 0.5
+
+    brace_orig_points = points - center
+    return brace_orig_points
+
+
+def get_brace_tip_point_index() -> int:
+    global brace_tip_point_index
+    if brace_tip_point_index is not None:
+        return brace_tip_point_index
+
+    points = get_brace_orig_points()
+    brace_tip_point_index = points[:, 1].argmin()
+
+    return brace_tip_point_index
+
+
+def get_brace_left_index() -> int:
+    global brace_left_index
+    if brace_left_index is not None:
+        return brace_left_index
+
+    points = get_brace_orig_points()
+    brace_left_index = points[:, 0].argmin()
+
+    return brace_left_index
+
+
+def get_brace_right_index() -> int:
+    global brace_left_index
+    if brace_left_index is not None:
+        return brace_left_index
+
+    points = get_brace_orig_points()
+    brace_left_index = points[:, 0].argmax()
+
+    return brace_left_index
```

### Comparing `janim-1.0.4/janim/items/svg/brace.svg` & `janim-1.1.0/janim/items/svg/brace.svg`

 * *Files 18% similar despite different names*

```diff
@@ -8,102 +8,101 @@
 00000070: 6c6e 733d 2268 7474 703a 2f2f 7777 772e  lns="http://www.
 00000080: 7733 2e6f 7267 2f32 3030 302f 7376 6722  w3.org/2000/svg"
 00000090: 2078 6d6c 6e73 3a78 6c69 6e6b 3d22 6874   xmlns:xlink="ht
 000000a0: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
 000000b0: 3139 3939 2f78 6c69 6e6b 2220 786d 6c6e  1999/xlink" xmln
 000000c0: 733a 6835 3d22 6874 7470 3a2f 2f77 7777  s:h5="http://www
 000000d0: 2e77 332e 6f72 672f 3139 3939 2f78 6874  .w3.org/1999/xht
-000000e0: 6d6c 223e 0d0a 2020 2020 3c67 3e0d 0a20  ml">..    <g>.. 
-000000f0: 2020 2020 2020 203c 6720 7472 616e 7366         <g transf
-00000100: 6f72 6d3d 2274 7261 6e73 6c61 7465 2832  orm="translate(2
-00000110: 3932 2e31 3338 3234 3939 3939 3939 3939  92.1382499999999
-00000120: 3720 3730 2e38 3636 3235 2922 3e0d 0a20  7 70.86625)">.. 
-00000130: 2020 2020 2020 2020 2020 203c 6720 636c             <g cl
-00000140: 6173 733d 2274 7970 7374 2d74 6578 7422  ass="typst-text"
-00000150: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
-00000160: 6528 312c 202d 3129 222f 3e0d 0a20 2020  e(1, -1)"/>..   
-00000170: 2020 2020 203c 2f67 3e0d 0a20 2020 2020       </g>..     
-00000180: 2020 203c 6720 7472 616e 7366 6f72 6d3d     <g transform=
-00000190: 2274 7261 6e73 6c61 7465 2832 3839 2e32  "translate(289.2
-000001a0: 3637 3235 2037 322e 3735 3832 3439 3939  6725 72.75824999
-000001b0: 3939 3939 3939 2922 3e0d 0a20 2020 2020  999999)">..     
-000001c0: 2020 2020 2020 203c 6720 636c 6173 733d         <g class=
-000001d0: 2274 7970 7374 2d74 6578 7422 2074 7261  "typst-text" tra
-000001e0: 6e73 666f 726d 3d22 7363 616c 6528 312c  nsform="scale(1,
-000001f0: 202d 3129 223e 0d0a 2020 2020 2020 2020   -1)">..        
-00000200: 2020 2020 2020 2020 3c75 7365 2078 6c69          <use xli
-00000210: 6e6b 3a68 7265 663d 2223 6744 3132 3833  nk:href="#gD1283
-00000220: 3637 4233 3938 4139 3644 4642 4241 3645  67B398A96DFBBA6E
-00000230: 4545 4342 4632 3835 4436 4222 2078 3d22  EECBF285D6B" x="
-00000240: 3022 2066 696c 6c3d 2223 6666 6666 6666  0" fill="#ffffff
-00000250: 222f 3e0d 0a20 2020 2020 2020 2020 2020  "/>..           
-00000260: 203c 2f67 3e0d 0a20 2020 2020 2020 203c   </g>..        <
-00000270: 2f67 3e0d 0a20 2020 203c 2f67 3e0d 0a20  /g>..    </g>.. 
-00000280: 2020 203c 6465 6673 2069 643d 2267 6c79     <defs id="gly
-00000290: 7068 223e 0d0a 2020 2020 2020 2020 3c73  ph">..        <s
-000002a0: 796d 626f 6c20 6964 3d22 6744 3132 3833  ymbol id="gD1283
-000002b0: 3637 4233 3938 4139 3644 4642 4241 3645  67B398A96DFBBA6E
-000002c0: 4545 4342 4632 3835 4436 4222 206f 7665  EECBF285D6B" ove
-000002d0: 7266 6c6f 773d 2276 6973 6962 6c65 223e  rflow="visible">
-000002e0: 0d0a 2020 2020 2020 2020 2020 2020 3c70  ..            <p
-000002f0: 6174 6820 643d 224d 2031 362e 3433 3420  ath d="M 16.434 
-00000300: 2d31 2e30 3132 204c 2031 362e 3433 3420  -1.012 L 16.434 
-00000310: 2d30 2e39 3739 2043 2031 362e 3433 3420  -0.979 C 16.434 
-00000320: 2d30 2e39 3032 2031 362e 3339 202d 302e  -0.902 16.39 -0.
-00000330: 3835 3820 3136 2e33 3133 202d 302e 3835  858 16.313 -0.85
-00000340: 3820 4320 3136 2e32 3538 202d 302e 3835  8 C 16.258 -0.85
-00000350: 3820 3136 2e32 3134 202d 302e 3838 2031  8 16.214 -0.88 1
-00000360: 362e 3139 3220 2d30 2e39 3335 2043 2031  6.192 -0.935 C 1
-00000370: 362e 3034 3920 2d31 2e33 3432 2031 352e  6.049 -1.342 15.
-00000380: 3731 3920 2d31 2e36 3631 2031 352e 3230  719 -1.661 15.20
-00000390: 3220 2d31 2e39 3033 2043 2031 342e 3735  2 -1.903 C 14.75
-000003a0: 3039 3939 202d 322e 3131 3220 3134 2e32  0999 -2.112 14.2
-000003b0: 3839 202d 322e 3231 3120 3133 2e38 3035  89 -2.211 13.805
-000003c0: 202d 322e 3231 3120 4c20 3130 2e37 3235   -2.211 L 10.725
-000003d0: 202d 322e 3231 3120 4320 392e 3538 3120   -2.211 C 9.581 
-000003e0: 2d32 2e32 3131 2038 2e35 3538 202d 322e  -2.211 8.558 -2.
-000003f0: 3739 3420 382e 3231 3720 2d33 2e35 3937  794 8.217 -3.597
-00000400: 2043 2038 2e30 3320 2d33 2e31 3436 2037   C 8.03 -3.146 7
-00000410: 2e36 3738 202d 322e 3830 3520 372e 3137  .678 -2.805 7.17
-00000420: 3220 2d32 2e35 3532 2043 2036 2e37 3231  2 -2.552 C 6.721
-00000430: 202d 322e 3332 3120 362e 3232 3620 2d32   -2.321 6.226 -2
-00000440: 2e32 3131 2035 2e37 3039 202d 322e 3231  .211 5.709 -2.21
-00000450: 3120 4c20 322e 3632 3920 2d32 2e32 3131  1 L 2.629 -2.211
-00000460: 2043 2032 2e31 3435 202d 322e 3231 3120   C 2.145 -2.211 
-00000470: 312e 3638 3320 2d32 2e31 3132 2031 2e32  1.683 -2.112 1.2
-00000480: 3332 202d 312e 3930 3320 4320 302e 3731  32 -1.903 C 0.71
-00000490: 3520 2d31 2e36 3631 2030 2e33 3835 202d  5 -1.661 0.385 -
-000004a0: 312e 3334 3220 302e 3234 3220 2d30 2e39  1.342 0.242 -0.9
-000004b0: 3335 2043 2030 2e32 3220 2d30 2e38 3820  35 C 0.22 -0.88 
-000004c0: 302e 3137 3620 2d30 2e38 3538 2030 2e31  0.176 -0.858 0.1
-000004d0: 3231 202d 302e 3835 3820 4320 302e 3034  21 -0.858 C 0.04
-000004e0: 3420 2d30 2e38 3538 2030 202d 302e 3930  4 -0.858 0 -0.90
-000004f0: 3220 3020 2d30 2e39 3739 204c 2030 202d  2 0 -0.979 L 0 -
-00000500: 312e 3031 3220 4320 302e 3138 3720 2d31  1.012 C 0.187 -1
-00000510: 2e35 3138 2030 2e35 3238 202d 312e 3935  .518 0.528 -1.95
-00000520: 3820 312e 3033 3420 2d32 2e33 3433 2043  8 1.034 -2.343 C
-00000530: 2031 2e35 3420 2d32 2e37 3238 2032 2e30   1.54 -2.728 2.0
-00000540: 3638 202d 322e 3931 3520 322e 3632 3920  68 -2.915 2.629 
-00000550: 2d32 2e39 3135 204c 2035 2e37 3039 202d  -2.915 L 5.709 -
-00000560: 322e 3931 3520 4320 362e 3234 3820 2d32  2.915 C 6.248 -2
-00000570: 2e39 3135 2036 2e37 3332 202d 322e 3939  .915 6.732 -2.99
-00000580: 3220 372e 3137 3220 2d33 2e31 3537 2043  2 7.172 -3.157 C
-00000590: 2037 2e37 3838 202d 332e 3337 3720 382e   7.788 -3.377 8.
-000005a0: 3039 3620 2d33 2e37 3037 2038 2e30 3936  096 -3.707 8.096
-000005b0: 202d 342e 3133 3620 4320 382e 3039 3620   -4.136 C 8.096 
-000005c0: 2d34 2e32 3133 2038 2e31 3420 2d34 2e32  -4.213 8.14 -4.2
-000005d0: 3537 2038 2e32 3137 202d 342e 3235 3720  57 8.217 -4.257 
-000005e0: 4320 382e 3239 3420 2d34 2e32 3537 2038  C 8.294 -4.257 8
-000005f0: 2e33 3338 202d 342e 3231 3320 382e 3333  .338 -4.213 8.33
-00000600: 3820 2d34 2e31 3336 2043 2038 2e33 3338  8 -4.136 C 8.338
-00000610: 202d 332e 3730 3720 382e 3634 3620 2d33   -3.707 8.646 -3
-00000620: 2e33 3737 2039 2e32 3632 202d 332e 3135  .377 9.262 -3.15
-00000630: 3720 4320 392e 3730 3220 2d32 2e39 3932  7 C 9.702 -2.992
-00000640: 2031 302e 3138 3620 2d32 2e39 3135 2031   10.186 -2.915 1
-00000650: 302e 3732 3520 2d32 2e39 3135 204c 2031  0.725 -2.915 L 1
-00000660: 332e 3830 3520 2d32 2e39 3135 2043 2031  3.805 -2.915 C 1
-00000670: 352e 3030 3420 2d32 2e39 3135 2031 362e  5.004 -2.915 16.
-00000680: 3039 3320 2d31 2e39 3134 2031 362e 3433  093 -1.914 16.43
-00000690: 3420 2d31 2e30 3132 205a 2022 2f3e 0d0a  4 -1.012 Z "/>..
-000006a0: 2020 2020 2020 2020 3c2f 7379 6d62 6f6c          </symbol
-000006b0: 3e0d 0a20 2020 203c 2f64 6566 733e 0d0a  >..    </defs>..
-000006c0: 3c2f 7376 673e 0d0a                      </svg>..
+000000e0: 6d6c 223e 0a20 2020 203c 673e 0a20 2020  ml">.    <g>.   
+000000f0: 2020 2020 203c 6720 7472 616e 7366 6f72       <g transfor
+00000100: 6d3d 2274 7261 6e73 6c61 7465 2832 3932  m="translate(292
+00000110: 2e31 3338 3234 3939 3939 3939 3939 3720  .13824999999997 
+00000120: 3730 2e38 3636 3235 2922 3e0a 2020 2020  70.86625)">.    
+00000130: 2020 2020 2020 2020 3c67 2063 6c61 7373          <g class
+00000140: 3d22 7479 7073 742d 7465 7874 2220 7472  ="typst-text" tr
+00000150: 616e 7366 6f72 6d3d 2273 6361 6c65 2831  ansform="scale(1
+00000160: 2c20 2d31 2922 2f3e 0a20 2020 2020 2020  , -1)"/>.       
+00000170: 203c 2f67 3e0a 2020 2020 2020 2020 3c67   </g>.        <g
+00000180: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00000190: 736c 6174 6528 3238 392e 3236 3732 3520  slate(289.26725 
+000001a0: 3732 2e37 3538 3234 3939 3939 3939 3939  72.7582499999999
+000001b0: 3929 223e 0a20 2020 2020 2020 2020 2020  9)">.           
+000001c0: 203c 6720 636c 6173 733d 2274 7970 7374   <g class="typst
+000001d0: 2d74 6578 7422 2074 7261 6e73 666f 726d  -text" transform
+000001e0: 3d22 7363 616c 6528 312c 202d 3129 223e  ="scale(1, -1)">
+000001f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000200: 203c 7573 6520 786c 696e 6b3a 6872 6566   <use xlink:href
+00000210: 3d22 2367 4431 3238 3336 3742 3339 3841  ="#gD128367B398A
+00000220: 3936 4446 4242 4136 4545 4543 4246 3238  96DFBBA6EEECBF28
+00000230: 3544 3642 2220 783d 2230 2220 6669 6c6c  5D6B" x="0" fill
+00000240: 3d22 2366 6666 6666 6622 2f3e 0a20 2020  ="#ffffff"/>.   
+00000250: 2020 2020 2020 2020 203c 2f67 3e0a 2020           </g>.  
+00000260: 2020 2020 2020 3c2f 673e 0a20 2020 203c        </g>.    <
+00000270: 2f67 3e0a 2020 2020 3c64 6566 7320 6964  /g>.    <defs id
+00000280: 3d22 676c 7970 6822 3e0a 2020 2020 2020  ="glyph">.      
+00000290: 2020 3c73 796d 626f 6c20 6964 3d22 6744    <symbol id="gD
+000002a0: 3132 3833 3637 4233 3938 4139 3644 4642  128367B398A96DFB
+000002b0: 4241 3645 4545 4342 4632 3835 4436 4222  BA6EEECBF285D6B"
+000002c0: 206f 7665 7266 6c6f 773d 2276 6973 6962   overflow="visib
+000002d0: 6c65 223e 0a20 2020 2020 2020 2020 2020  le">.           
+000002e0: 203c 7061 7468 2064 3d22 4d20 3136 2e34   <path d="M 16.4
+000002f0: 3334 202d 312e 3031 3220 4c20 3136 2e34  34 -1.012 L 16.4
+00000300: 3334 202d 302e 3937 3920 4320 3136 2e34  34 -0.979 C 16.4
+00000310: 3334 202d 302e 3930 3220 3136 2e33 3920  34 -0.902 16.39 
+00000320: 2d30 2e38 3538 2031 362e 3331 3320 2d30  -0.858 16.313 -0
+00000330: 2e38 3538 2043 2031 362e 3235 3820 2d30  .858 C 16.258 -0
+00000340: 2e38 3538 2031 362e 3231 3420 2d30 2e38  .858 16.214 -0.8
+00000350: 3820 3136 2e31 3932 202d 302e 3933 3520  8 16.192 -0.935 
+00000360: 4320 3136 2e30 3439 202d 312e 3334 3220  C 16.049 -1.342 
+00000370: 3135 2e37 3139 202d 312e 3636 3120 3135  15.719 -1.661 15
+00000380: 2e32 3032 202d 312e 3930 3320 4320 3134  .202 -1.903 C 14
+00000390: 2e37 3530 3939 3920 2d32 2e31 3132 2031  .750999 -2.112 1
+000003a0: 342e 3238 3920 2d32 2e32 3131 2031 332e  4.289 -2.211 13.
+000003b0: 3830 3520 2d32 2e32 3131 204c 2031 302e  805 -2.211 L 10.
+000003c0: 3732 3520 2d32 2e32 3131 2043 2039 2e35  725 -2.211 C 9.5
+000003d0: 3831 202d 322e 3231 3120 382e 3535 3820  81 -2.211 8.558 
+000003e0: 2d32 2e37 3934 2038 2e32 3137 202d 332e  -2.794 8.217 -3.
+000003f0: 3539 3720 4320 382e 3033 202d 332e 3134  597 C 8.03 -3.14
+00000400: 3620 372e 3637 3820 2d32 2e38 3035 2037  6 7.678 -2.805 7
+00000410: 2e31 3732 202d 322e 3535 3220 4320 362e  .172 -2.552 C 6.
+00000420: 3732 3120 2d32 2e33 3231 2036 2e32 3236  721 -2.321 6.226
+00000430: 202d 322e 3231 3120 352e 3730 3920 2d32   -2.211 5.709 -2
+00000440: 2e32 3131 204c 2032 2e36 3239 202d 322e  .211 L 2.629 -2.
+00000450: 3231 3120 4320 322e 3134 3520 2d32 2e32  211 C 2.145 -2.2
+00000460: 3131 2031 2e36 3833 202d 322e 3131 3220  11 1.683 -2.112 
+00000470: 312e 3233 3220 2d31 2e39 3033 2043 2030  1.232 -1.903 C 0
+00000480: 2e37 3135 202d 312e 3636 3120 302e 3338  .715 -1.661 0.38
+00000490: 3520 2d31 2e33 3432 2030 2e32 3432 202d  5 -1.342 0.242 -
+000004a0: 302e 3933 3520 4320 302e 3232 202d 302e  0.935 C 0.22 -0.
+000004b0: 3838 2030 2e31 3736 202d 302e 3835 3820  88 0.176 -0.858 
+000004c0: 302e 3132 3120 2d30 2e38 3538 2043 2030  0.121 -0.858 C 0
+000004d0: 2e30 3434 202d 302e 3835 3820 3020 2d30  .044 -0.858 0 -0
+000004e0: 2e39 3032 2030 202d 302e 3937 3920 4c20  .902 0 -0.979 L 
+000004f0: 3020 2d31 2e30 3132 2043 2030 2e31 3837  0 -1.012 C 0.187
+00000500: 202d 312e 3531 3820 302e 3532 3820 2d31   -1.518 0.528 -1
+00000510: 2e39 3538 2031 2e30 3334 202d 322e 3334  .958 1.034 -2.34
+00000520: 3320 4320 312e 3534 202d 322e 3732 3820  3 C 1.54 -2.728 
+00000530: 322e 3036 3820 2d32 2e39 3135 2032 2e36  2.068 -2.915 2.6
+00000540: 3239 202d 322e 3931 3520 4c20 352e 3730  29 -2.915 L 5.70
+00000550: 3920 2d32 2e39 3135 2043 2036 2e32 3438  9 -2.915 C 6.248
+00000560: 202d 322e 3931 3520 362e 3733 3220 2d32   -2.915 6.732 -2
+00000570: 2e39 3932 2037 2e31 3732 202d 332e 3135  .992 7.172 -3.15
+00000580: 3720 4320 372e 3738 3820 2d33 2e33 3737  7 C 7.788 -3.377
+00000590: 2038 2e30 3936 202d 332e 3730 3720 382e   8.096 -3.707 8.
+000005a0: 3039 3620 2d34 2e31 3336 2043 2038 2e30  096 -4.136 C 8.0
+000005b0: 3936 202d 342e 3231 3320 382e 3134 202d  96 -4.213 8.14 -
+000005c0: 342e 3235 3720 382e 3231 3720 2d34 2e32  4.257 8.217 -4.2
+000005d0: 3537 2043 2038 2e32 3934 202d 342e 3235  57 C 8.294 -4.25
+000005e0: 3720 382e 3333 3820 2d34 2e32 3133 2038  7 8.338 -4.213 8
+000005f0: 2e33 3338 202d 342e 3133 3620 4320 382e  .338 -4.136 C 8.
+00000600: 3333 3820 2d33 2e37 3037 2038 2e36 3436  338 -3.707 8.646
+00000610: 202d 332e 3337 3720 392e 3236 3220 2d33   -3.377 9.262 -3
+00000620: 2e31 3537 2043 2039 2e37 3032 202d 322e  .157 C 9.702 -2.
+00000630: 3939 3220 3130 2e31 3836 202d 322e 3931  992 10.186 -2.91
+00000640: 3520 3130 2e37 3235 202d 322e 3931 3520  5 10.725 -2.915 
+00000650: 4c20 3133 2e38 3035 202d 322e 3931 3520  L 13.805 -2.915 
+00000660: 4320 3135 2e30 3034 202d 322e 3931 3520  C 15.004 -2.915 
+00000670: 3136 2e30 3933 202d 312e 3931 3420 3136  16.093 -1.914 16
+00000680: 2e34 3334 202d 312e 3031 3220 5a20 222f  .434 -1.012 Z "/
+00000690: 3e0a 2020 2020 2020 2020 3c2f 7379 6d62  >.        </symb
+000006a0: 6f6c 3e0a 2020 2020 3c2f 6465 6673 3e0a  ol>.    </defs>.
+000006b0: 3c2f 7376 673e 0a                        </svg>.
```

### Comparing `janim-1.0.4/janim/items/svg/svg_item.py` & `janim-1.1.0/janim/items/svg/svg_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,277 +1,269 @@
-00000000: 0d0a 696d 706f 7274 206f 730d 0a66 726f  ..import os..fro
-00000010: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00000020: 4361 6c6c 6162 6c65 0d0a 0d0a 696d 706f  Callable....impo
-00000030: 7274 206e 756d 7079 2061 7320 6e70 0d0a  rt numpy as np..
-00000040: 696d 706f 7274 2073 7667 656c 656d 656e  import svgelemen
-00000050: 7473 2061 7320 7365 0d0a 0d0a 6672 6f6d  ts as se....from
-00000060: 206a 616e 696d 2e63 6f6e 7374 616e 7473   janim.constants
-00000070: 2069 6d70 6f72 7420 4f52 4947 494e 2c20   import ORIGIN, 
-00000080: 5249 4748 540d 0a66 726f 6d20 6a61 6e69  RIGHT..from jani
-00000090: 6d2e 6974 656d 732e 6974 656d 2069 6d70  m.items.item imp
-000000a0: 6f72 7420 4974 656d 0d0a 6672 6f6d 206a  ort Item..from j
-000000b0: 616e 696d 2e69 7465 6d73 2e70 6f69 6e74  anim.items.point
-000000c0: 7320 696d 706f 7274 2047 726f 7570 0d0a  s import Group..
-000000d0: 6672 6f6d 206a 616e 696d 2e69 7465 6d73  from janim.items
-000000e0: 2e76 6974 656d 2069 6d70 6f72 7420 5649  .vitem import VI
-000000f0: 7465 6d0d 0a66 726f 6d20 6a61 6e69 6d2e  tem..from janim.
-00000100: 6c6f 6767 6572 2069 6d70 6f72 7420 6c6f  logger import lo
-00000110: 670d 0a66 726f 6d20 6a61 6e69 6d2e 7574  g..from janim.ut
-00000120: 696c 732e 6265 7a69 6572 2069 6d70 6f72  ils.bezier impor
-00000130: 7420 5061 7468 4275 696c 6465 720d 0a66  t PathBuilder..f
-00000140: 726f 6d20 6a61 6e69 6d2e 7574 696c 732e  rom janim.utils.
-00000150: 636f 6e66 6967 2069 6d70 6f72 7420 436f  config import Co
-00000160: 6e66 6967 0d0a 6672 6f6d 206a 616e 696d  nfig..from janim
-00000170: 2e75 7469 6c73 2e66 696c 655f 6f70 7320  .utils.file_ops 
-00000180: 696d 706f 7274 2066 696e 645f 6669 6c65  import find_file
-00000190: 0d0a 0d0a 2320 e8bf 99e9 878c e79a 8420  ....# ......... 
-000001a0: 332e 3237 3220 e698 afe6 898b e58a a8e8  3.272 ..........
-000001b0: af95 e587 bae6 9da5 e79a 840d 0a44 4546  .............DEF
-000001c0: 4155 4c54 5f53 5647 4954 454d 5f53 4341  AULT_SVGITEM_SCA
-000001d0: 4c45 5f46 4143 544f 5220 3d20 332e 3237  LE_FACTOR = 3.27
-000001e0: 320d 0a53 5452 4f4b 455f 5749 4454 485f  2..STROKE_WIDTH_
-000001f0: 434f 4e56 4552 5349 4f4e 203d 2030 2e30  CONVERSION = 0.0
-00000200: 310d 0a0d 0a74 7970 6520 5649 7465 6d42  1....type VItemB
-00000210: 7569 6c64 6572 203d 2043 616c 6c61 626c  uilder = Callabl
-00000220: 655b 5b5d 2c20 5649 7465 6d5d 0d0a 0d0a  e[[], VItem]....
-00000230: 0d0a 6465 6620 5f63 6f6e 7665 7274 5f70  ..def _convert_p
-00000240: 6f69 6e74 5f74 6f5f 3364 2878 3a20 666c  oint_to_3d(x: fl
-00000250: 6f61 742c 2079 3a20 666c 6f61 7429 202d  oat, y: float) -
-00000260: 3e20 6e70 2e6e 6461 7272 6179 3a0d 0a20  > np.ndarray:.. 
-00000270: 2020 2072 6574 7572 6e20 6e70 2e61 7272     return np.arr
-00000280: 6179 285b 782c 2079 2c20 305d 290d 0a0d  ay([x, y, 0])...
-00000290: 0a0d 0a64 6566 205f 636f 6e76 6572 745f  ...def _convert_
-000002a0: 6f70 6163 6974 7928 783a 2066 6c6f 6174  opacity(x: float
-000002b0: 207c 204e 6f6e 6529 202d 3e20 666c 6f61   | None) -> floa
-000002c0: 743a 0d0a 2020 2020 7265 7475 726e 2030  t:..    return 0
-000002d0: 2e20 6966 2078 2069 7320 4e6f 6e65 2065  . if x is None e
-000002e0: 6c73 6520 780d 0a0d 0a0d 0a63 6c61 7373  lse x......class
-000002f0: 2053 5647 4974 656d 2847 726f 7570 5b56   SVGItem(Group[V
-00000300: 4974 656d 5d29 3a0d 0a20 2020 2027 2727  Item]):..    '''
-00000310: 0d0a 2020 2020 e4bc a0e5 85a5 2053 5647  ..    ...... SVG
-00000320: 20e6 9687 e4bb b6e8 b7af e5be 84ef bc8c   ...............
-00000330: e8a7 a3e6 9e90 e4b8 bae7 89a9 e4bb b60d  ................
-00000340: 0a20 2020 2027 2727 0d0a 2020 2020 7376  .    '''..    sv
-00000350: 675f 7061 7274 5f64 6566 6175 6c74 5f6b  g_part_default_k
-00000360: 7761 7267 7320 3d20 6469 6374 280d 0a20  wargs = dict(.. 
-00000370: 2020 2020 2020 2073 7472 6f6b 655f 7261         stroke_ra
-00000380: 6469 7573 3d31 2e30 202a 2053 5452 4f4b  dius=1.0 * STROK
-00000390: 455f 5749 4454 485f 434f 4e56 4552 5349  E_WIDTH_CONVERSI
-000003a0: 4f4e 202f 2032 2c0d 0a20 2020 2020 2020  ON / 2,..       
-000003b0: 2073 7472 6f6b 655f 636f 6c6f 723d 4e6f   stroke_color=No
-000003c0: 6e65 2c0d 0a20 2020 2020 2020 2073 7472  ne,..        str
-000003d0: 6f6b 655f 616c 7068 613d 302c 0d0a 2020  oke_alpha=0,..  
-000003e0: 2020 2020 2020 6669 6c6c 5f63 6f6c 6f72        fill_color
-000003f0: 3d4e 6f6e 652c 0d0a 2020 2020 2020 2020  =None,..        
-00000400: 6669 6c6c 5f61 6c70 6861 3d30 0d0a 2020  fill_alpha=0..  
-00000410: 2020 290d 0a20 2020 2076 6974 656d 5f62    )..    vitem_b
-00000420: 7569 6c64 6572 735f 6d61 703a 2064 6963  uilders_map: dic
-00000430: 745b 7475 706c 652c 206c 6973 745b 5649  t[tuple, list[VI
-00000440: 7465 6d42 7569 6c64 6572 5d5d 203d 207b  temBuilder]] = {
-00000450: 7d0d 0a0d 0a20 2020 2064 6566 205f 5f69  }....    def __i
-00000460: 6e69 745f 5f28 7365 6c66 2c20 6669 6c65  nit__(self, file
-00000470: 5f70 6174 683a 2073 7472 2c20 2a2a 6b77  _path: str, **kw
-00000480: 6172 6773 293a 0d0a 2020 2020 2020 2020  args):..        
-00000490: 6974 656d 7320 3d20 7365 6c66 2e67 6574  items = self.get
-000004a0: 5f69 7465 6d73 5f66 726f 6d5f 6669 6c65  _items_from_file
-000004b0: 2866 696c 655f 7061 7468 290d 0a0d 0a20  (file_path).... 
-000004c0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
-000004d0: 5f69 6e69 745f 5f28 2a69 7465 6d73 2c20  _init__(*items, 
-000004e0: 2a2a 6b77 6172 6773 290d 0a0d 0a20 2020  **kwargs)....   
-000004f0: 2020 2020 2073 656c 6628 5649 7465 6d29       self(VItem)
-00000500: 2e70 6f69 6e74 732e 7363 616c 6528 0d0a  .points.scale(..
-00000510: 2020 2020 2020 2020 2020 2020 436f 6e66              Conf
-00000520: 6967 2e67 6574 2e70 6978 656c 5f74 6f5f  ig.get.pixel_to_
-00000530: 6672 616d 655f 7261 7469 6f20 2a20 4445  frame_ratio * DE
-00000540: 4641 554c 545f 5356 4749 5445 4d5f 5343  FAULT_SVGITEM_SC
-00000550: 414c 455f 4641 4354 4f52 2c0d 0a20 2020  ALE_FACTOR,..   
-00000560: 2020 2020 2020 2020 2061 626f 7574 5f70           about_p
-00000570: 6f69 6e74 3d4f 5249 4749 4e0d 0a20 2020  oint=ORIGIN..   
-00000580: 2020 2020 2029 2e66 6c69 7028 5249 4748       ).flip(RIGH
-00000590: 5429 0d0a 0d0a 2020 2020 2020 2020 7365  T)....        se
-000005a0: 6c66 2e6d 6f76 655f 696e 746f 5f70 6f73  lf.move_into_pos
-000005b0: 6974 696f 6e28 290d 0a0d 0a20 2020 2064  ition()....    d
-000005c0: 6566 206d 6f76 655f 696e 746f 5f70 6f73  ef move_into_pos
-000005d0: 6974 696f 6e28 7365 6c66 2920 2d3e 204e  ition(self) -> N
-000005e0: 6f6e 653a 0d0a 2020 2020 2020 2020 7061  one:..        pa
-000005f0: 7373 0d0a 0d0a 2020 2020 4073 7461 7469  ss....    @stati
-00000600: 636d 6574 686f 640d 0a20 2020 2064 6566  cmethod..    def
-00000610: 2067 6574 5f69 7465 6d73 5f66 726f 6d5f   get_items_from_
-00000620: 6669 6c65 2866 696c 655f 7061 7468 3a20  file(file_path: 
-00000630: 7374 7229 202d 3e20 6c69 7374 5b49 7465  str) -> list[Ite
-00000640: 6d5d 3a0d 0a20 2020 2020 2020 2027 2727  m]:..        '''
-00000650: 0d0a 2020 2020 2020 2020 e8a7 a3e6 9e90  ..        ......
-00000660: e696 87e4 bbb6 e5b9 b6e5 be97 e588 b0e7  ................
-00000670: 89a9 e4bb b6e5 8897 e8a1 a80d 0a20 2020  .............   
-00000680: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-00000690: 2020 6669 6c65 5f70 6174 6820 3d20 6669    file_path = fi
-000006a0: 6e64 5f66 696c 6528 6669 6c65 5f70 6174  nd_file(file_pat
-000006b0: 6829 0d0a 2020 2020 2020 2020 6d74 696d  h)..        mtim
-000006c0: 6520 3d20 6f73 2e70 6174 682e 6765 746d  e = os.path.getm
-000006d0: 7469 6d65 2866 696c 655f 7061 7468 290d  time(file_path).
-000006e0: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
-000006f0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
-00000700: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
-00000710: 6528 6669 6c65 5f70 6174 6829 295b 305d  e(file_path))[0]
-00000720: 0d0a 2020 2020 2020 2020 6b65 7920 3d20  ..        key = 
-00000730: 286e 616d 652c 206d 7469 6d65 290d 0a0d  (name, mtime)...
-00000740: 0a20 2020 2020 2020 2063 6163 6865 6420  .        cached 
-00000750: 3d20 5356 4749 7465 6d2e 7669 7465 6d5f  = SVGItem.vitem_
-00000760: 6275 696c 6465 7273 5f6d 6170 2e67 6574  builders_map.get
-00000770: 286b 6579 2c20 4e6f 6e65 290d 0a20 2020  (key, None)..   
-00000780: 2020 2020 2069 6620 6361 6368 6564 2069       if cached i
-00000790: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-000007a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000007b0: 5b62 7569 6c64 6572 2829 2066 6f72 2062  [builder() for b
-000007c0: 7569 6c64 6572 2069 6e20 6361 6368 6564  uilder in cached
-000007d0: 5d0d 0a0d 0a20 2020 2020 2020 2073 7667  ]....        svg
-000007e0: 3a20 7365 2e53 5647 203d 2073 652e 5356  : se.SVG = se.SV
-000007f0: 472e 7061 7273 6528 6669 6c65 5f70 6174  G.parse(file_pat
-00000800: 6829 0d0a 0d0a 2020 2020 2020 2020 6f66  h)....        of
-00000810: 6673 6574 203d 206e 702e 6172 7261 7928  fset = np.array(
-00000820: 5b73 7667 2e77 6964 7468 202f 202d 322c  [svg.width / -2,
-00000830: 2073 7667 2e68 6569 6768 7420 2f20 2d32   svg.height / -2
-00000840: 5d29 0d0a 0d0a 2020 2020 2020 2020 6275  ])....        bu
-00000850: 696c 6465 7273 3a20 6c69 7374 5b56 4974  ilders: list[VIt
-00000860: 656d 4275 696c 6465 725d 203d 205b 5d0d  emBuilder] = [].
-00000870: 0a20 2020 2020 2020 2066 6f72 2073 6861  .        for sha
-00000880: 7065 2069 6e20 7376 672e 656c 656d 656e  pe in svg.elemen
-00000890: 7473 2829 3a0d 0a20 2020 2020 2020 2020  ts():..         
-000008a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000008b0: 2873 6861 7065 2c20 2873 652e 4772 6f75  (shape, (se.Grou
-000008c0: 702c 2073 652e 5573 6529 293a 0d0a 2020  p, se.Use)):..  
-000008d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000008e0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-000008f0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00000900: 6e63 6528 7368 6170 652c 2073 652e 5061  nce(shape, se.Pa
-00000910: 7468 293a 0d0a 2020 2020 2020 2020 2020  th):..          
-00000920: 2020 2020 2020 6275 696c 6465 7273 2e61        builders.a
-00000930: 7070 656e 6428 5356 4749 7465 6d2e 636f  ppend(SVGItem.co
-00000940: 6e76 6572 745f 7061 7468 2873 6861 7065  nvert_path(shape
-00000950: 2c20 6f66 6673 6574 2929 0d0a 2020 2020  , offset))..    
-00000960: 2020 2020 2020 2020 656c 6966 2074 7970          elif typ
-00000970: 6528 7368 6170 6529 2069 7320 7365 2e53  e(shape) is se.S
-00000980: 5647 456c 656d 656e 743a 0d0a 2020 2020  VGElement:..    
-00000990: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000009a0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-000009b0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000009c0: 2020 2020 2020 2020 206c 6f67 2e77 6172           log.war
-000009d0: 6e69 6e67 2866 2755 6e73 7570 706f 7274  ning(f'Unsupport
-000009e0: 6564 2065 6c65 6d65 6e74 2074 7970 653a  ed element type:
-000009f0: 207b 7479 7065 2873 6861 7065 297d 2729   {type(shape)}')
-00000a00: 0d0a 0d0a 2020 2020 2020 2020 5356 4749  ....        SVGI
-00000a10: 7465 6d2e 7669 7465 6d5f 6275 696c 6465  tem.vitem_builde
-00000a20: 7273 5f6d 6170 5b6b 6579 5d20 3d20 6275  rs_map[key] = bu
-00000a30: 696c 6465 7273 0d0a 2020 2020 2020 2020  ilders..        
-00000a40: 7265 7475 726e 205b 6275 696c 6465 7228  return [builder(
-00000a50: 2920 666f 7220 6275 696c 6465 7220 696e  ) for builder in
-00000a60: 2062 7569 6c64 6572 735d 0d0a 0d0a 2020   builders]....  
-00000a70: 2020 4073 7461 7469 636d 6574 686f 640d    @staticmethod.
-00000a80: 0a20 2020 2064 6566 2063 6f6e 7665 7274  .    def convert
-00000a90: 5f70 6174 6828 7061 7468 3a20 7365 2e50  _path(path: se.P
-00000aa0: 6174 682c 206f 6666 7365 743a 206e 702e  ath, offset: np.
-00000ab0: 6e64 6172 7261 7929 202d 3e20 5649 7465  ndarray) -> VIte
-00000ac0: 6d42 7569 6c64 6572 3a0d 0a20 2020 2020  mBuilder:..     
-00000ad0: 2020 2062 7569 6c64 6572 203d 2050 6174     builder = Pat
-00000ae0: 6842 7569 6c64 6572 2829 0d0a 2020 2020  hBuilder()..    
-00000af0: 2020 2020 7365 676d 656e 745f 636c 6173      segment_clas
-00000b00: 735f 746f 5f66 756e 635f 6d61 7020 3d20  s_to_func_map = 
-00000b10: 7b0d 0a20 2020 2020 2020 2020 2020 2073  {..            s
-00000b20: 652e 4d6f 7665 3a20 2862 7569 6c64 6572  e.Move: (builder
-00000b30: 2e6d 6f76 655f 746f 2c20 2827 656e 6427  .move_to, ('end'
-00000b40: 2c29 292c 0d0a 2020 2020 2020 2020 2020  ,)),..          
-00000b50: 2020 7365 2e43 6c6f 7365 3a20 2862 7569    se.Close: (bui
-00000b60: 6c64 6572 2e63 6c6f 7365 5f70 6174 682c  lder.close_path,
-00000b70: 2028 2929 2c0d 0a20 2020 2020 2020 2020   ()),..         
-00000b80: 2020 2073 652e 4c69 6e65 3a20 2862 7569     se.Line: (bui
-00000b90: 6c64 6572 2e6c 696e 655f 746f 2c20 2827  lder.line_to, ('
-00000ba0: 656e 6427 2c29 292c 0d0a 2020 2020 2020  end',)),..      
-00000bb0: 2020 2020 2020 7365 2e51 7561 6472 6174        se.Quadrat
-00000bc0: 6963 4265 7a69 6572 3a20 2862 7569 6c64  icBezier: (build
-00000bd0: 6572 2e63 6f6e 6963 5f74 6f2c 2028 2763  er.conic_to, ('c
-00000be0: 6f6e 7472 6f6c 272c 2027 656e 6427 2929  ontrol', 'end'))
-00000bf0: 2c0d 0a20 2020 2020 2020 2020 2020 2073  ,..            s
-00000c00: 652e 4375 6269 6342 657a 6965 723a 2028  e.CubicBezier: (
-00000c10: 6275 696c 6465 722e 6375 6269 635f 746f  builder.cubic_to
-00000c20: 2c20 2827 636f 6e74 726f 6c31 272c 2027  , ('control1', '
-00000c30: 636f 6e74 726f 6c32 272c 2027 656e 6427  control2', 'end'
-00000c40: 2929 2c0d 0a20 2020 2020 2020 2020 2020  )),..           
-00000c50: 2073 652e 4172 633a 2028 6c61 6d62 6461   se.Arc: (lambda
-00000c60: 2073 6567 6d65 6e74 3a20 6275 696c 6465   segment: builde
-00000c70: 722e 6172 635f 746f 285f 636f 6e76 6572  r.arc_to(_conver
-00000c80: 745f 706f 696e 745f 746f 5f33 6428 2a73  t_point_to_3d(*s
-00000c90: 6567 6d65 6e74 2e65 6e64 292c 2073 6567  egment.end), seg
-00000ca0: 6d65 6e74 2e73 7765 6570 292c 204e 6f6e  ment.sweep), Non
-00000cb0: 6529 2c0d 0a20 2020 2020 2020 207d 0d0a  e),..        }..
-00000cc0: 0d0a 2020 2020 2020 2020 666f 7220 7365  ..        for se
-00000cd0: 676d 656e 7420 696e 2070 6174 683a 0d0a  gment in path:..
-00000ce0: 2020 2020 2020 2020 2020 2020 7365 676d              segm
-00000cf0: 656e 745f 636c 6173 7320 3d20 7365 676d  ent_class = segm
-00000d00: 656e 742e 5f5f 636c 6173 735f 5f0d 0a20  ent.__class__.. 
-00000d10: 2020 2020 2020 2020 2020 2066 756e 632c             func,
-00000d20: 2061 7474 725f 6e61 6d65 7320 3d20 7365   attr_names = se
-00000d30: 676d 656e 745f 636c 6173 735f 746f 5f66  gment_class_to_f
-00000d40: 756e 635f 6d61 705b 7365 676d 656e 745f  unc_map[segment_
-00000d50: 636c 6173 735d 0d0a 2020 2020 2020 2020  class]..        
-00000d60: 2020 2020 6966 2061 7474 725f 6e61 6d65      if attr_name
-00000d70: 7320 6973 204e 6f6e 653a 0d0a 2020 2020  s is None:..    
-00000d80: 2020 2020 2020 2020 2020 2020 6675 6e63              func
-00000d90: 2873 6567 6d65 6e74 290d 0a20 2020 2020  (segment)..     
-00000da0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00000db0: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00000dc0: 696e 7473 203d 205b 0d0a 2020 2020 2020  ints = [..      
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 5f63                _c
-00000de0: 6f6e 7665 7274 5f70 6f69 6e74 5f74 6f5f  onvert_point_to_
-00000df0: 3364 282a 6765 7461 7474 7228 7365 676d  3d(*getattr(segm
-00000e00: 656e 742c 2061 7474 725f 6e61 6d65 2929  ent, attr_name))
-00000e10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000e20: 2020 2020 2020 666f 7220 6174 7472 5f6e        for attr_n
-00000e30: 616d 6520 696e 2061 7474 725f 6e61 6d65  ame in attr_name
-00000e40: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00000e50: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
-00000e60: 2020 2020 2020 6675 6e63 282a 706f 696e        func(*poin
-00000e70: 7473 290d 0a0d 0a20 2020 2020 2020 206f  ts)....        o
-00000e80: 7061 6369 7479 203d 2066 6c6f 6174 2870  pacity = float(p
-00000e90: 6174 682e 7661 6c75 6573 2e67 6574 2827  ath.values.get('
-00000ea0: 6f70 6163 6974 7927 2c20 3129 290d 0a0d  opacity', 1))...
-00000eb0: 0a20 2020 2020 2020 2076 6974 656d 5f73  .        vitem_s
-00000ec0: 7479 6c65 7320 3d20 6469 6374 280d 0a20  tyles = dict(.. 
-00000ed0: 2020 2020 2020 2020 2020 2073 7472 6f6b             strok
-00000ee0: 655f 7261 6469 7573 3d70 6174 682e 7374  e_radius=path.st
-00000ef0: 726f 6b65 5f77 6964 7468 202a 2053 5452  roke_width * STR
-00000f00: 4f4b 455f 5749 4454 485f 434f 4e56 4552  OKE_WIDTH_CONVER
-00000f10: 5349 4f4e 202f 2032 2c0d 0a20 2020 2020  SION / 2,..     
-00000f20: 2020 2020 2020 2073 7472 6f6b 655f 636f         stroke_co
-00000f30: 6c6f 723d 7061 7468 2e73 7472 6f6b 652e  lor=path.stroke.
-00000f40: 6865 782c 0d0a 2020 2020 2020 2020 2020  hex,..          
-00000f50: 2020 7374 726f 6b65 5f61 6c70 6861 3d5f    stroke_alpha=_
-00000f60: 636f 6e76 6572 745f 6f70 6163 6974 7928  convert_opacity(
-00000f70: 7061 7468 2e73 7472 6f6b 652e 6f70 6163  path.stroke.opac
-00000f80: 6974 7929 202a 206f 7061 6369 7479 2c0d  ity) * opacity,.
-00000f90: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00000fa0: 6c5f 636f 6c6f 723d 7061 7468 2e66 696c  l_color=path.fil
-00000fb0: 6c2e 6865 782c 0d0a 2020 2020 2020 2020  l.hex,..        
-00000fc0: 2020 2020 6669 6c6c 5f61 6c70 6861 3d5f      fill_alpha=_
-00000fd0: 636f 6e76 6572 745f 6f70 6163 6974 7928  convert_opacity(
-00000fe0: 7061 7468 2e66 696c 6c2e 6f70 6163 6974  path.fill.opacit
-00000ff0: 7929 202a 206f 7061 6369 7479 0d0a 2020  y) * opacity..  
-00001000: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00001010: 2076 6974 656d 5f70 6f69 6e74 7320 3d20   vitem_points = 
-00001020: 6275 696c 6465 722e 6765 7428 290d 0a20  builder.get().. 
-00001030: 2020 2020 2020 2076 6974 656d 5f70 6f69         vitem_poi
-00001040: 6e74 735b 3a2c 203a 325d 202b 3d20 6f66  nts[:, :2] += of
-00001050: 6673 6574 0d0a 0d0a 2020 2020 2020 2020  fset....        
-00001060: 6465 6620 7669 7465 6d5f 6275 696c 6465  def vitem_builde
-00001070: 7228 2920 2d3e 2056 4974 656d 3a0d 0a20  r() -> VItem:.. 
-00001080: 2020 2020 2020 2020 2020 2076 6974 656d             vitem
-00001090: 203d 2056 4974 656d 282a 2a53 5647 4974   = VItem(**SVGIt
-000010a0: 656d 2e73 7667 5f70 6172 745f 6465 6661  em.svg_part_defa
-000010b0: 756c 745f 6b77 6172 6773 290d 0a20 2020  ult_kwargs)..   
-000010c0: 2020 2020 2020 2020 2076 6974 656d 2e73           vitem.s
-000010d0: 6574 5f73 7479 6c65 282a 2a76 6974 656d  et_style(**vitem
-000010e0: 5f73 7479 6c65 7329 0d0a 2020 2020 2020  _styles)..      
-000010f0: 2020 2020 2020 7669 7465 6d2e 706f 696e        vitem.poin
-00001100: 7473 2e73 6574 2876 6974 656d 5f70 6f69  ts.set(vitem_poi
-00001110: 6e74 7329 0d0a 2020 2020 2020 2020 2020  nts)..          
-00001120: 2020 7265 7475 726e 2076 6974 656d 0d0a    return vitem..
-00001130: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001140: 2076 6974 656d 5f62 7569 6c64 6572 0d0a   vitem_builder..
+00000000: 0a69 6d70 6f72 7420 6f73 0a66 726f 6d20  .import os.from 
+00000010: 7479 7069 6e67 2069 6d70 6f72 7420 4361  typing import Ca
+00000020: 6c6c 6162 6c65 0a0a 696d 706f 7274 206e  llable..import n
+00000030: 756d 7079 2061 7320 6e70 0a69 6d70 6f72  umpy as np.impor
+00000040: 7420 7376 6765 6c65 6d65 6e74 7320 6173  t svgelements as
+00000050: 2073 650a 0a66 726f 6d20 6a61 6e69 6d2e   se..from janim.
+00000060: 636f 6e73 7461 6e74 7320 696d 706f 7274  constants import
+00000070: 204f 5249 4749 4e2c 2052 4947 4854 0a66   ORIGIN, RIGHT.f
+00000080: 726f 6d20 6a61 6e69 6d2e 6974 656d 732e  rom janim.items.
+00000090: 6974 656d 2069 6d70 6f72 7420 4974 656d  item import Item
+000000a0: 0a66 726f 6d20 6a61 6e69 6d2e 6974 656d  .from janim.item
+000000b0: 732e 706f 696e 7473 2069 6d70 6f72 7420  s.points import 
+000000c0: 4772 6f75 700a 6672 6f6d 206a 616e 696d  Group.from janim
+000000d0: 2e69 7465 6d73 2e76 6974 656d 2069 6d70  .items.vitem imp
+000000e0: 6f72 7420 5649 7465 6d0a 6672 6f6d 206a  ort VItem.from j
+000000f0: 616e 696d 2e6c 6f67 6765 7220 696d 706f  anim.logger impo
+00000100: 7274 206c 6f67 0a66 726f 6d20 6a61 6e69  rt log.from jani
+00000110: 6d2e 7574 696c 732e 6265 7a69 6572 2069  m.utils.bezier i
+00000120: 6d70 6f72 7420 5061 7468 4275 696c 6465  mport PathBuilde
+00000130: 720a 6672 6f6d 206a 616e 696d 2e75 7469  r.from janim.uti
+00000140: 6c73 2e63 6f6e 6669 6720 696d 706f 7274  ls.config import
+00000150: 2043 6f6e 6669 670a 6672 6f6d 206a 616e   Config.from jan
+00000160: 696d 2e75 7469 6c73 2e66 696c 655f 6f70  im.utils.file_op
+00000170: 7320 696d 706f 7274 2066 696e 645f 6669  s import find_fi
+00000180: 6c65 0a0a 2320 e8bf 99e9 878c e79a 8420  le..# ......... 
+00000190: 332e 3237 3220 e698 afe6 898b e58a a8e8  3.272 ..........
+000001a0: af95 e587 bae6 9da5 e79a 840a 4445 4641  ............DEFA
+000001b0: 554c 545f 5356 4749 5445 4d5f 5343 414c  ULT_SVGITEM_SCAL
+000001c0: 455f 4641 4354 4f52 203d 2033 2e32 3732  E_FACTOR = 3.272
+000001d0: 0a53 5452 4f4b 455f 5749 4454 485f 434f  .STROKE_WIDTH_CO
+000001e0: 4e56 4552 5349 4f4e 203d 2030 2e30 310a  NVERSION = 0.01.
+000001f0: 0a74 7970 6520 5649 7465 6d42 7569 6c64  .type VItemBuild
+00000200: 6572 203d 2043 616c 6c61 626c 655b 5b5d  er = Callable[[]
+00000210: 2c20 5649 7465 6d5d 0a0a 0a64 6566 205f  , VItem]...def _
+00000220: 636f 6e76 6572 745f 706f 696e 745f 746f  convert_point_to
+00000230: 5f33 6428 783a 2066 6c6f 6174 2c20 793a  _3d(x: float, y:
+00000240: 2066 6c6f 6174 2920 2d3e 206e 702e 6e64   float) -> np.nd
+00000250: 6172 7261 793a 0a20 2020 2072 6574 7572  array:.    retur
+00000260: 6e20 6e70 2e61 7272 6179 285b 782c 2079  n np.array([x, y
+00000270: 2c20 305d 290a 0a0a 6465 6620 5f63 6f6e  , 0])...def _con
+00000280: 7665 7274 5f6f 7061 6369 7479 2878 3a20  vert_opacity(x: 
+00000290: 666c 6f61 7420 7c20 4e6f 6e65 2920 2d3e  float | None) ->
+000002a0: 2066 6c6f 6174 3a0a 2020 2020 7265 7475   float:.    retu
+000002b0: 726e 2030 2e20 6966 2078 2069 7320 4e6f  rn 0. if x is No
+000002c0: 6e65 2065 6c73 6520 780a 0a0a 636c 6173  ne else x...clas
+000002d0: 7320 5356 4749 7465 6d28 4772 6f75 705b  s SVGItem(Group[
+000002e0: 5649 7465 6d5d 293a 0a20 2020 2027 2727  VItem]):.    '''
+000002f0: 0a20 2020 20e4 bca0 e585 a520 5356 4720  .    ...... SVG 
+00000300: e696 87e4 bbb6 e8b7 afe5 be84 efbc 8ce8  ................
+00000310: a7a3 e69e 90e4 b8ba e789 a9e4 bbb6 0a20  ............... 
+00000320: 2020 2027 2727 0a20 2020 2073 7667 5f70     '''.    svg_p
+00000330: 6172 745f 6465 6661 756c 745f 6b77 6172  art_default_kwar
+00000340: 6773 203d 2064 6963 7428 0a20 2020 2020  gs = dict(.     
+00000350: 2020 2073 7472 6f6b 655f 7261 6469 7573     stroke_radius
+00000360: 3d31 2e30 202a 2053 5452 4f4b 455f 5749  =1.0 * STROKE_WI
+00000370: 4454 485f 434f 4e56 4552 5349 4f4e 202f  DTH_CONVERSION /
+00000380: 2032 2c0a 2020 2020 2020 2020 7374 726f   2,.        stro
+00000390: 6b65 5f63 6f6c 6f72 3d4e 6f6e 652c 0a20  ke_color=None,. 
+000003a0: 2020 2020 2020 2073 7472 6f6b 655f 616c         stroke_al
+000003b0: 7068 613d 302c 0a20 2020 2020 2020 2066  pha=0,.        f
+000003c0: 696c 6c5f 636f 6c6f 723d 4e6f 6e65 2c0a  ill_color=None,.
+000003d0: 2020 2020 2020 2020 6669 6c6c 5f61 6c70          fill_alp
+000003e0: 6861 3d30 0a20 2020 2029 0a20 2020 2076  ha=0.    ).    v
+000003f0: 6974 656d 5f62 7569 6c64 6572 735f 6d61  item_builders_ma
+00000400: 703a 2064 6963 745b 7475 706c 652c 206c  p: dict[tuple, l
+00000410: 6973 745b 5649 7465 6d42 7569 6c64 6572  ist[VItemBuilder
+00000420: 5d5d 203d 207b 7d0a 0a20 2020 2064 6566  ]] = {}..    def
+00000430: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00000440: 6669 6c65 5f70 6174 683a 2073 7472 2c20  file_path: str, 
+00000450: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00000460: 2020 2069 7465 6d73 203d 2073 656c 662e     items = self.
+00000470: 6765 745f 6974 656d 735f 6672 6f6d 5f66  get_items_from_f
+00000480: 696c 6528 6669 6c65 5f70 6174 6829 0a0a  ile(file_path)..
+00000490: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+000004a0: 5f5f 696e 6974 5f5f 282a 6974 656d 732c  __init__(*items,
+000004b0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+000004c0: 2020 2020 7365 6c66 2856 4974 656d 292e      self(VItem).
+000004d0: 706f 696e 7473 2e73 6361 6c65 280a 2020  points.scale(.  
+000004e0: 2020 2020 2020 2020 2020 436f 6e66 6967            Config
+000004f0: 2e67 6574 2e70 6978 656c 5f74 6f5f 6672  .get.pixel_to_fr
+00000500: 616d 655f 7261 7469 6f20 2a20 4445 4641  ame_ratio * DEFA
+00000510: 554c 545f 5356 4749 5445 4d5f 5343 414c  ULT_SVGITEM_SCAL
+00000520: 455f 4641 4354 4f52 2c0a 2020 2020 2020  E_FACTOR,.      
+00000530: 2020 2020 2020 6162 6f75 745f 706f 696e        about_poin
+00000540: 743d 4f52 4947 494e 0a20 2020 2020 2020  t=ORIGIN.       
+00000550: 2029 2e66 6c69 7028 5249 4748 5429 0a0a   ).flip(RIGHT)..
+00000560: 2020 2020 2020 2020 7365 6c66 2e6d 6f76          self.mov
+00000570: 655f 696e 746f 5f70 6f73 6974 696f 6e28  e_into_position(
+00000580: 290a 0a20 2020 2064 6566 206d 6f76 655f  )..    def move_
+00000590: 696e 746f 5f70 6f73 6974 696f 6e28 7365  into_position(se
+000005a0: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
+000005b0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+000005c0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+000005d0: 2064 6566 2067 6574 5f69 7465 6d73 5f66   def get_items_f
+000005e0: 726f 6d5f 6669 6c65 2866 696c 655f 7061  rom_file(file_pa
+000005f0: 7468 3a20 7374 7229 202d 3e20 6c69 7374  th: str) -> list
+00000600: 5b49 7465 6d5d 3a0a 2020 2020 2020 2020  [Item]:.        
+00000610: 2727 270a 2020 2020 2020 2020 e8a7 a3e6  '''.        ....
+00000620: 9e90 e696 87e4 bbb6 e5b9 b6e5 be97 e588  ................
+00000630: b0e7 89a9 e4bb b6e5 8897 e8a1 a80a 2020  ..............  
+00000640: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00000650: 2020 6669 6c65 5f70 6174 6820 3d20 6669    file_path = fi
+00000660: 6e64 5f66 696c 6528 6669 6c65 5f70 6174  nd_file(file_pat
+00000670: 6829 0a20 2020 2020 2020 206d 7469 6d65  h).        mtime
+00000680: 203d 206f 732e 7061 7468 2e67 6574 6d74   = os.path.getmt
+00000690: 696d 6528 6669 6c65 5f70 6174 6829 0a20  ime(file_path). 
+000006a0: 2020 2020 2020 206e 616d 6520 3d20 6f73         name = os
+000006b0: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+000006c0: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+000006d0: 6669 6c65 5f70 6174 6829 295b 305d 0a20  file_path))[0]. 
+000006e0: 2020 2020 2020 206b 6579 203d 2028 6e61         key = (na
+000006f0: 6d65 2c20 6d74 696d 6529 0a0a 2020 2020  me, mtime)..    
+00000700: 2020 2020 6361 6368 6564 203d 2053 5647      cached = SVG
+00000710: 4974 656d 2e76 6974 656d 5f62 7569 6c64  Item.vitem_build
+00000720: 6572 735f 6d61 702e 6765 7428 6b65 792c  ers_map.get(key,
+00000730: 204e 6f6e 6529 0a20 2020 2020 2020 2069   None).        i
+00000740: 6620 6361 6368 6564 2069 7320 6e6f 7420  f cached is not 
+00000750: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00000760: 2020 7265 7475 726e 205b 6275 696c 6465    return [builde
+00000770: 7228 2920 666f 7220 6275 696c 6465 7220  r() for builder 
+00000780: 696e 2063 6163 6865 645d 0a0a 2020 2020  in cached]..    
+00000790: 2020 2020 7376 673a 2073 652e 5356 4720      svg: se.SVG 
+000007a0: 3d20 7365 2e53 5647 2e70 6172 7365 2866  = se.SVG.parse(f
+000007b0: 696c 655f 7061 7468 290a 0a20 2020 2020  ile_path)..     
+000007c0: 2020 206f 6666 7365 7420 3d20 6e70 2e61     offset = np.a
+000007d0: 7272 6179 285b 7376 672e 7769 6474 6820  rray([svg.width 
+000007e0: 2f20 2d32 2c20 7376 672e 6865 6967 6874  / -2, svg.height
+000007f0: 202f 202d 325d 290a 0a20 2020 2020 2020   / -2])..       
+00000800: 2062 7569 6c64 6572 733a 206c 6973 745b   builders: list[
+00000810: 5649 7465 6d42 7569 6c64 6572 5d20 3d20  VItemBuilder] = 
+00000820: 5b5d 0a20 2020 2020 2020 2066 6f72 2073  [].        for s
+00000830: 6861 7065 2069 6e20 7376 672e 656c 656d  hape in svg.elem
+00000840: 656e 7473 2829 3a0a 2020 2020 2020 2020  ents():.        
+00000850: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00000860: 6528 7368 6170 652c 2028 7365 2e47 726f  e(shape, (se.Gro
+00000870: 7570 2c20 7365 2e55 7365 2929 3a0a 2020  up, se.Use)):.  
+00000880: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000890: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+000008a0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+000008b0: 6365 2873 6861 7065 2c20 7365 2e50 6174  ce(shape, se.Pat
+000008c0: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+000008d0: 2020 2020 6275 696c 6465 7273 2e61 7070      builders.app
+000008e0: 656e 6428 5356 4749 7465 6d2e 636f 6e76  end(SVGItem.conv
+000008f0: 6572 745f 7061 7468 2873 6861 7065 2c20  ert_path(shape, 
+00000900: 6f66 6673 6574 2929 0a20 2020 2020 2020  offset)).       
+00000910: 2020 2020 2065 6c69 6620 7479 7065 2873       elif type(s
+00000920: 6861 7065 2920 6973 2073 652e 5356 4745  hape) is se.SVGE
+00000930: 6c65 6d65 6e74 3a0a 2020 2020 2020 2020  lement:.        
+00000940: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00000950: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00000960: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00000970: 2020 206c 6f67 2e77 6172 6e69 6e67 2866     log.warning(f
+00000980: 2755 6e73 7570 706f 7274 6564 2065 6c65  'Unsupported ele
+00000990: 6d65 6e74 2074 7970 653a 207b 7479 7065  ment type: {type
+000009a0: 2873 6861 7065 297d 2729 0a0a 2020 2020  (shape)}')..    
+000009b0: 2020 2020 5356 4749 7465 6d2e 7669 7465      SVGItem.vite
+000009c0: 6d5f 6275 696c 6465 7273 5f6d 6170 5b6b  m_builders_map[k
+000009d0: 6579 5d20 3d20 6275 696c 6465 7273 0a20  ey] = builders. 
+000009e0: 2020 2020 2020 2072 6574 7572 6e20 5b62         return [b
+000009f0: 7569 6c64 6572 2829 2066 6f72 2062 7569  uilder() for bui
+00000a00: 6c64 6572 2069 6e20 6275 696c 6465 7273  lder in builders
+00000a10: 5d0a 0a20 2020 2040 7374 6174 6963 6d65  ]..    @staticme
+00000a20: 7468 6f64 0a20 2020 2064 6566 2063 6f6e  thod.    def con
+00000a30: 7665 7274 5f70 6174 6828 7061 7468 3a20  vert_path(path: 
+00000a40: 7365 2e50 6174 682c 206f 6666 7365 743a  se.Path, offset:
+00000a50: 206e 702e 6e64 6172 7261 7929 202d 3e20   np.ndarray) -> 
+00000a60: 5649 7465 6d42 7569 6c64 6572 3a0a 2020  VItemBuilder:.  
+00000a70: 2020 2020 2020 6275 696c 6465 7220 3d20        builder = 
+00000a80: 5061 7468 4275 696c 6465 7228 290a 2020  PathBuilder().  
+00000a90: 2020 2020 2020 7365 676d 656e 745f 636c        segment_cl
+00000aa0: 6173 735f 746f 5f66 756e 635f 6d61 7020  ass_to_func_map 
+00000ab0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00000ac0: 7365 2e4d 6f76 653a 2028 6275 696c 6465  se.Move: (builde
+00000ad0: 722e 6d6f 7665 5f74 6f2c 2028 2765 6e64  r.move_to, ('end
+00000ae0: 272c 2929 2c0a 2020 2020 2020 2020 2020  ',)),.          
+00000af0: 2020 7365 2e43 6c6f 7365 3a20 2862 7569    se.Close: (bui
+00000b00: 6c64 6572 2e63 6c6f 7365 5f70 6174 682c  lder.close_path,
+00000b10: 2028 2929 2c0a 2020 2020 2020 2020 2020   ()),.          
+00000b20: 2020 7365 2e4c 696e 653a 2028 6275 696c    se.Line: (buil
+00000b30: 6465 722e 6c69 6e65 5f74 6f2c 2028 2765  der.line_to, ('e
+00000b40: 6e64 272c 2929 2c0a 2020 2020 2020 2020  nd',)),.        
+00000b50: 2020 2020 7365 2e51 7561 6472 6174 6963      se.Quadratic
+00000b60: 4265 7a69 6572 3a20 2862 7569 6c64 6572  Bezier: (builder
+00000b70: 2e63 6f6e 6963 5f74 6f2c 2028 2763 6f6e  .conic_to, ('con
+00000b80: 7472 6f6c 272c 2027 656e 6427 2929 2c0a  trol', 'end')),.
+00000b90: 2020 2020 2020 2020 2020 2020 7365 2e43              se.C
+00000ba0: 7562 6963 4265 7a69 6572 3a20 2862 7569  ubicBezier: (bui
+00000bb0: 6c64 6572 2e63 7562 6963 5f74 6f2c 2028  lder.cubic_to, (
+00000bc0: 2763 6f6e 7472 6f6c 3127 2c20 2763 6f6e  'control1', 'con
+00000bd0: 7472 6f6c 3227 2c20 2765 6e64 2729 292c  trol2', 'end')),
+00000be0: 0a20 2020 2020 2020 2020 2020 2073 652e  .            se.
+00000bf0: 4172 633a 2028 6c61 6d62 6461 2073 6567  Arc: (lambda seg
+00000c00: 6d65 6e74 3a20 6275 696c 6465 722e 6172  ment: builder.ar
+00000c10: 635f 746f 285f 636f 6e76 6572 745f 706f  c_to(_convert_po
+00000c20: 696e 745f 746f 5f33 6428 2a73 6567 6d65  int_to_3d(*segme
+00000c30: 6e74 2e65 6e64 292c 2073 6567 6d65 6e74  nt.end), segment
+00000c40: 2e73 7765 6570 292c 204e 6f6e 6529 2c0a  .sweep), None),.
+00000c50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00000c60: 2020 2066 6f72 2073 6567 6d65 6e74 2069     for segment i
+00000c70: 6e20 7061 7468 3a0a 2020 2020 2020 2020  n path:.        
+00000c80: 2020 2020 7365 676d 656e 745f 636c 6173      segment_clas
+00000c90: 7320 3d20 7365 676d 656e 742e 5f5f 636c  s = segment.__cl
+00000ca0: 6173 735f 5f0a 2020 2020 2020 2020 2020  ass__.          
+00000cb0: 2020 6675 6e63 2c20 6174 7472 5f6e 616d    func, attr_nam
+00000cc0: 6573 203d 2073 6567 6d65 6e74 5f63 6c61  es = segment_cla
+00000cd0: 7373 5f74 6f5f 6675 6e63 5f6d 6170 5b73  ss_to_func_map[s
+00000ce0: 6567 6d65 6e74 5f63 6c61 7373 5d0a 2020  egment_class].  
+00000cf0: 2020 2020 2020 2020 2020 6966 2061 7474            if att
+00000d00: 725f 6e61 6d65 7320 6973 204e 6f6e 653a  r_names is None:
+00000d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d20: 2066 756e 6328 7365 676d 656e 7429 0a20   func(segment). 
+00000d30: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00000d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d50: 2070 6f69 6e74 7320 3d20 5b0a 2020 2020   points = [.    
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 5f63 6f6e 7665 7274 5f70 6f69 6e74 5f74  _convert_point_t
+00000d80: 6f5f 3364 282a 6765 7461 7474 7228 7365  o_3d(*getattr(se
+00000d90: 676d 656e 742c 2061 7474 725f 6e61 6d65  gment, attr_name
+00000da0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00000db0: 2020 2020 2020 2066 6f72 2061 7474 725f         for attr_
+00000dc0: 6e61 6d65 2069 6e20 6174 7472 5f6e 616d  name in attr_nam
+00000dd0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00000de0: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+00000df0: 2020 2020 2066 756e 6328 2a70 6f69 6e74       func(*point
+00000e00: 7329 0a0a 2020 2020 2020 2020 6f70 6163  s)..        opac
+00000e10: 6974 7920 3d20 666c 6f61 7428 7061 7468  ity = float(path
+00000e20: 2e76 616c 7565 732e 6765 7428 276f 7061  .values.get('opa
+00000e30: 6369 7479 272c 2031 2929 0a0a 2020 2020  city', 1))..    
+00000e40: 2020 2020 7669 7465 6d5f 7374 796c 6573      vitem_styles
+00000e50: 203d 2064 6963 7428 0a20 2020 2020 2020   = dict(.       
+00000e60: 2020 2020 2073 7472 6f6b 655f 7261 6469       stroke_radi
+00000e70: 7573 3d70 6174 682e 7374 726f 6b65 5f77  us=path.stroke_w
+00000e80: 6964 7468 202a 2053 5452 4f4b 455f 5749  idth * STROKE_WI
+00000e90: 4454 485f 434f 4e56 4552 5349 4f4e 202f  DTH_CONVERSION /
+00000ea0: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+00000eb0: 7374 726f 6b65 5f63 6f6c 6f72 3d70 6174  stroke_color=pat
+00000ec0: 682e 7374 726f 6b65 2e68 6578 2c0a 2020  h.stroke.hex,.  
+00000ed0: 2020 2020 2020 2020 2020 7374 726f 6b65            stroke
+00000ee0: 5f61 6c70 6861 3d5f 636f 6e76 6572 745f  _alpha=_convert_
+00000ef0: 6f70 6163 6974 7928 7061 7468 2e73 7472  opacity(path.str
+00000f00: 6f6b 652e 6f70 6163 6974 7929 202a 206f  oke.opacity) * o
+00000f10: 7061 6369 7479 2c0a 2020 2020 2020 2020  pacity,.        
+00000f20: 2020 2020 6669 6c6c 5f63 6f6c 6f72 3d70      fill_color=p
+00000f30: 6174 682e 6669 6c6c 2e68 6578 2c0a 2020  ath.fill.hex,.  
+00000f40: 2020 2020 2020 2020 2020 6669 6c6c 5f61            fill_a
+00000f50: 6c70 6861 3d5f 636f 6e76 6572 745f 6f70  lpha=_convert_op
+00000f60: 6163 6974 7928 7061 7468 2e66 696c 6c2e  acity(path.fill.
+00000f70: 6f70 6163 6974 7929 202a 206f 7061 6369  opacity) * opaci
+00000f80: 7479 0a20 2020 2020 2020 2029 0a20 2020  ty.        ).   
+00000f90: 2020 2020 2076 6974 656d 5f70 6f69 6e74       vitem_point
+00000fa0: 7320 3d20 6275 696c 6465 722e 6765 7428  s = builder.get(
+00000fb0: 290a 2020 2020 2020 2020 7669 7465 6d5f  ).        vitem_
+00000fc0: 706f 696e 7473 5b3a 2c20 3a32 5d20 2b3d  points[:, :2] +=
+00000fd0: 206f 6666 7365 740a 0a20 2020 2020 2020   offset..       
+00000fe0: 2064 6566 2076 6974 656d 5f62 7569 6c64   def vitem_build
+00000ff0: 6572 2829 202d 3e20 5649 7465 6d3a 0a20  er() -> VItem:. 
+00001000: 2020 2020 2020 2020 2020 2076 6974 656d             vitem
+00001010: 203d 2056 4974 656d 282a 2a53 5647 4974   = VItem(**SVGIt
+00001020: 656d 2e73 7667 5f70 6172 745f 6465 6661  em.svg_part_defa
+00001030: 756c 745f 6b77 6172 6773 290a 2020 2020  ult_kwargs).    
+00001040: 2020 2020 2020 2020 7669 7465 6d2e 7365          vitem.se
+00001050: 745f 7374 796c 6528 2a2a 7669 7465 6d5f  t_style(**vitem_
+00001060: 7374 796c 6573 290a 2020 2020 2020 2020  styles).        
+00001070: 2020 2020 7669 7465 6d2e 706f 696e 7473      vitem.points
+00001080: 2e73 6574 2876 6974 656d 5f70 6f69 6e74  .set(vitem_point
+00001090: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
+000010a0: 6574 7572 6e20 7669 7465 6d0a 0a20 2020  eturn vitem..   
+000010b0: 2020 2020 2072 6574 7572 6e20 7669 7465       return vite
+000010c0: 6d5f 6275 696c 6465 720a                 m_builder.
```

### Comparing `janim-1.0.4/janim/items/text/text.py` & `janim-1.1.0/janim/items/text/text.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,493 +1,493 @@
-from __future__ import annotations
-
-import inspect
-import itertools as it
-import re
-from collections import defaultdict
-from enum import Enum
-from typing import Any, Callable, Concatenate, Iterable, Self
-
-import numpy as np
-
-from janim.components.points import Cmpt_Points
-from janim.constants import (DOWN, GREY, LEFT, MED_SMALL_BUFF, ORIGIN, RIGHT,
-                             UL, UP)
-from janim.exception import ColorNotFoundError
-from janim.items.geometry.line import Line
-from janim.items.points import Group, Points
-from janim.items.vitem import VItem
-from janim.logger import log
-from janim.typing import JAnimColor
-from janim.utils.config import Config
-from janim.utils.font import Font, get_fontpath_by_name
-from janim.utils.simple_functions import decode_utf8
-from janim.utils.space_ops import get_norm, normalize
-
-DEFAULT_FONT_SIZE = 24
-ORIG_FONT_SIZE = 48
-
-
-def _get_color_value(key: str) -> JAnimColor:
-    '''
-    根据 ``key`` 从 ``janim.constants.colors`` 得到颜色
-
-    如果 ``key`` 以 ``#`` 开头，则直接返回原值
-    '''
-    if key.startswith('#'):
-        return key
-
-    import janim.constants.colors as colors
-    if not hasattr(colors, key):
-        raise ColorNotFoundError(f'No built-in color named {key}')
-    return getattr(colors, key)
-
-
-type ActConverter = Callable[[str], Any]
-type ActCaller = Callable[Concatenate[TextChar, ...], Any]
-type Act = tuple[Iterable[ActConverter], ActCaller]
-type ActName = str
-
-type ActParams = Iterable[str]
-type ActParamsStack = list[ActParams]
-
-type ActAt = int
-type ActStart = tuple[ActName, ActParams]
-type ActEnd = str
-
-available_act_map: dict[ActName, list[Act]] = defaultdict(list)
-
-
-def _register_acts(names: list[ActName], *acts: Act) -> None:
-    '''
-    用于声明可用的富文本格式
-    '''
-    for name in names:
-        available_act_map[name].extend(acts)
-
-
-_register_acts(
-    ['color', 'c'],
-    ((_get_color_value,),           lambda char, color: char.color.set(color)),
-    ((float, float, float),         lambda char, r, g, b: char.color.set([r, g, b])),
-    ((float, float, float, float),  lambda char, r, g, b, a: char.color.set_rgbas([[r, g, b, a]]))
-)
-_register_acts(
-    ['stroke_color', 'sc'],
-    ((_get_color_value,),           lambda char, color: char.stroke.set(color)),
-    ((float, float, float),         lambda char, r, g, b: char.stroke.set([r, g, b])),
-    ((float, float, float, float),  lambda char, r, g, b, a: char.stroke.set_rgbas([[r, g, b, a]]))
-)
-_register_acts(
-    ['fill_color', 'fc'],
-    ((_get_color_value,),           lambda char, color: char.fill.set(color)),
-    ((float, float, float),         lambda char, r, g, b: char.fill.set([r, g, b])),
-    ((float, float, float, float),  lambda char, r, g, b, a: char.fill.set_rgbas([[r, g, b, a]]))
-)
-_register_acts(
-    ['alpha', 'a'],
-    ((float,), lambda char, a: char.color.set(alpha=a))
-)
-_register_acts(
-    ['stroke_alpha', 'sa'],
-    ((float,), lambda char, a: char.stroke.set(alpha=a))
-)
-_register_acts(
-    ['fill_alpha', 'fa'],
-    ((float,), lambda char, a: char.fill.set(alpha=a))
-)
-_register_acts(
-    ['stroke', 's'],
-    ((float,), lambda char, radius: char.radius.set(radius))
-)
-_register_acts(
-    ['font_scale', 'fs'],
-    ((float,), lambda char, factor: char.points.scale(factor, about_point=ORIGIN))
-)
-
-
-class TextChar(VItem):
-    '''
-    字符物件，作为 :class:`TextLine` 的子物件，在创建 :class:`TextLine` 时产生
-    '''
-    def __init__(
-        self,
-        char: str,
-        fonts: list[Font],
-        font_size: float,
-        fill_alpha=None,
-        **kwargs
-    ):
-        super().__init__(fill_alpha=fill_alpha, **kwargs)
-        self.char = char
-
-        unicode = decode_utf8(char)
-        font_render = self.get_font_for_render(unicode, fonts)
-
-        outline, advance = font_render.get_glyph_data(unicode)
-
-        font_scale_factor = font_size / ORIG_FONT_SIZE
-        frame_scale_factor = Config.get.pixel_to_frame_ratio / 32
-        scale_factor = font_scale_factor * frame_scale_factor
-
-        self.points.set(outline * scale_factor)
-
-        # 标记位置
-        self.mark = Points(
-            ORIGIN, RIGHT * font_scale_factor, UP * font_scale_factor,
-            [advance[0] * scale_factor, advance[1] * scale_factor, 0]
-        )
-        Cmpt_Points.apply_points_fn.connect(
-            self.points,
-            lambda func, about_point: self.mark.points.apply_points_fn(func,
-                                                                       about_point=about_point,
-                                                                       about_edge=None)
-        )
-
-    @staticmethod
-    def get_font_for_render(unicode: str, fonts: list[Font]) -> Font:
-        '''
-        从字体列表中找到支持显示 ``unicode`` 的字体，如果找不到只好选用第一个
-        '''
-        font_render = fonts[0]
-        for font in fonts:
-            idx = font.face.get_char_index(unicode)
-            if idx != 0:
-                font_render = font
-                break
-        return font_render
-
-    def get_mark_orig(self) -> np.ndarray:
-        return self.mark.points._points.data[0]
-
-    def get_mark_right(self) -> np.ndarray:
-        return self.mark.points._points.data[1]
-
-    def get_mark_up(self) -> np.ndarray:
-        return self.mark.points._points.data[2]
-
-    def get_mark_advance(self) -> np.ndarray:
-        return self.mark.points._points.data[3]
-
-    def get_advance_length(self) -> float:
-        return get_norm(self.get_mark_advance() - self.get_mark_orig())
-
-    def apply_act_list(self, act_params_map: dict[str, ActParamsStack]) -> None:
-        '''
-        应用富文本样式，由 :meth:`Text.apply_rich_text` 调用
-        '''
-        for name, params_stack in act_params_map.items():
-            params = params_stack[-1]
-            for converters, caller in available_act_map[name]:
-                if len(converters) == len(params):
-                    try:
-                        caller(
-                            self, *[
-                                converter(param)
-                                for converter, param in zip(converters, params)
-                            ]
-                        )
-                    except Exception:
-                        log.error(f'应用 {name} 时，{params} 与 {[cvt.__name__ for cvt in converters]} 不匹配')
-                        raise
-
-                    break
-            else:
-                txt = ','.join([
-                    '[' + ','.join([cvt.__name__ for cvt in act[0]]) + ']'
-                    for act in available_act_map[name]
-                ])
-                log.warning(f'应用 "{name}" 时，{params} 与 {txt} 没有匹配项')
-
-
-class TextLine(VItem, Group[TextChar]):
-    '''
-    单行文字物件，作为 :class:`Text` 的子物件，在创建 :class:`Text` 时产生s
-    '''
-    def __init__(
-        self,
-        text: str,
-        fonts: list[Font],
-        font_size: float,
-        char_kwargs={},
-        fill_alpha=None,
-        **kwargs
-    ):
-        self.text = text
-
-        super().__init__(
-            *[
-                TextChar(char, fonts, font_size, **char_kwargs)
-                for char in text
-            ],
-            fill_alpha=fill_alpha,
-            **kwargs
-        )
-
-        # 标记位置
-        self.mark = Points(ORIGIN, RIGHT, UP)
-        self.mark.points.scale(font_size / ORIG_FONT_SIZE, about_point=ORIGIN)
-        Cmpt_Points.apply_points_fn.connect(
-            self.points,
-            lambda func, about_point: self.mark.points.apply_points_fn(func,
-                                                                       about_point=about_point,
-                                                                       about_edge=None)
-        )
-
-    def get_mark_orig(self) -> np.ndarray:
-        return self.mark.points._points.data[0]
-
-    def get_mark_right(self) -> np.ndarray:
-        return self.mark.points._points.data[1]
-
-    def get_mark_up(self) -> np.ndarray:
-        return self.mark.points._points.data[2]
-
-    def arrange_in_line(self, buff: float = 0) -> Self:
-        '''
-        根据 ``advance`` 的标记信息排列该行
-        '''
-        if len(self.children) == 0:
-            return
-
-        pos = None
-
-        for i, char in enumerate(self):
-            if i != 0:
-                char.points.shift(pos - char.get_mark_orig())
-
-            orig = char.get_mark_orig()
-            advance = char.get_mark_advance()
-            pos = advance if buff == 0 else advance + buff * normalize(advance - orig)
-
-        return self
-
-
-class Text(VItem, Group[TextLine]):
-    '''
-    文字物件
-    '''
-    class Format(Enum):
-        PlainText = 0
-        RichText = 1
-
-    def __init__(
-        self,
-        text: str,
-        font: str | Iterable[str] = [],
-        font_size: float = DEFAULT_FONT_SIZE,
-        format: Format = Format.PlainText,
-        line_kwargs: dict = {},
-        stroke_alpha: float = 0,
-        fill_alpha: float = 1,
-        **kwargs
-    ) -> None:
-        # 获取字体
-        if isinstance(font, str):
-            font = [font]
-
-        cfg_font = Config.get.font
-        if isinstance(cfg_font, str):
-            font.append(cfg_font)
-        else:
-            font.extend(cfg_font)
-
-        fonts = [
-            Font.get(get_fontpath_by_name(name))
-            for name in font
-        ]
-
-        if format is not Text.Format.RichText:
-            self.text = text
-        else:
-            # 如果是 RichText，获取属性列表
-            self.text = ''
-            self.act_params_list: list[tuple[ActAt, ActStart | ActEnd]] = []
-            idx = 0
-            iter = re.finditer(r'(<+)(/?[^<]*?)>', text)
-            for match in iter:
-                match: re.Match
-                start, end = match.span()
-                left, mid = match.group(1, 2)
-
-                self.text += text[idx:start]
-                idx = end
-
-                left_cnt = len(left)
-                self.text += '<' * (left_cnt // 2)
-                if left_cnt % 2 == 0:
-                    self.text += mid + '>'
-                else:
-                    if mid.startswith('/'):
-                        self.act_params_list.append((len(self.text), mid[1:]))
-                    else:
-                        split = mid.split()
-                        self.act_params_list.append((len(self.text), (split[0], split[1:])))
-
-            self.text += text[idx:]
-
-        super().__init__(
-            *[
-                TextLine(line_text, fonts=fonts, font_size=font_size, **line_kwargs)
-                for line_text in self.text.split('\n')
-            ],
-            stroke_alpha=stroke_alpha,
-            fill_alpha=fill_alpha,
-            **kwargs
-        )
-
-        if format is Text.Format.RichText:
-            self.apply_rich_text()
-        for line in self.children:
-            line.arrange_in_line()
-        self.arrange_in_lines()
-        self.astype(Points).points.to_center()
-
-    def is_null(self) -> bool:
-        return True
-
-    def idx_to_row_col(self, idx: int) -> tuple[int, int]:
-        '''
-        由字符索引得到 行数、列数 索引
-        '''
-        for i, line in enumerate(self):
-            if idx < len(line):
-                return i, idx
-            idx -= len(line)
-        return len(self) - 1, idx
-
-    def select_parts(self, pattern):
-        '''
-        根据 ``pattern`` 获得文字中的部分
-        '''
-        total_text: str = ''.join([line.text for line in self])
-        parts = []
-        for mch in re.finditer(pattern, total_text):
-            l_row, l_col = self.idx_to_row_col(mch.start())
-            r_row, r_col = self.idx_to_row_col(mch.end())
-            if l_row == r_row:
-                parts.append(self[l_row][l_col:r_col])
-            else:
-                parts.append(
-                    Group(*it.chain(
-                        self[l_row][l_col:],
-                        *self[l_row + 1: r_row],
-                        self[r_row][:r_col]
-                    ))
-                )
-        return Group(*parts)
-
-    def arrange_in_lines(self, buff: float = 0, base_buff: float = 0.85) -> Self:
-        '''
-        - ``buff``: 每行之间的额外间距
-        - ``base_buff``: 每行之间的基本间距，默认值 ``0.85`` 用于将两行上下排列，如果是 ``0`` 则会让两行完全重合，大部分时候不需要传入该值
-        '''
-        if len(self.children) == 0:
-            return
-
-        pos = self.children[0].get_mark_orig()
-        for line in self.children[1:]:
-            vert = line.get_mark_orig() - line.get_mark_up()
-            target = pos + base_buff * vert + buff * normalize(vert)
-            line.points.shift(
-                target - line.get_mark_orig()
-            )
-            pos = line.get_mark_orig()
-
-        return self
-
-    # TODO: word_wrap
-    # 使用 TypstDoc 可以轻松做到
-    # 我感觉可以不用给 Text 实现这功能了
-
-    def apply_rich_text(self) -> None:
-        '''
-        应用富文本效果
-        '''
-        text_at = 0
-        act_idx = 0
-        act_params_map: defaultdict[str, ActParamsStack] = defaultdict(list)
-        for line in self.children:
-            for char in line.children:
-                while act_idx < len(self.act_params_list):
-                    next_act_at, next_act = self.act_params_list[act_idx]
-                    if text_at < next_act_at:
-                        break
-
-                    if isinstance(next_act, str):   # ActEnd
-                        stack = act_params_map[next_act]
-                        stack.pop()
-                        if not stack:
-                            del act_params_map[next_act]
-                    else:   # ActStart
-                        name, params = next_act
-                        act_params_map[name].append(params)
-
-                    act_idx += 1
-
-                char.apply_act_list(act_params_map)
-                text_at += 1
-
-            text_at += 1
-
-
-class Title(Group):
-    '''
-    标题
-
-    - ``include_underline=True`` 会添加下划线（默认添加）
-    - ``underline_width`` 下划线的长度（默认屏幕宽 - 2 个单位）
-    - ``match_underline_width_to_text=True`` 时将下划线的长度和文字匹配（默认为 ``False``）
-    '''
-    def __init__(
-        self,
-        text: str,
-        font: str | Iterable[str] = [],
-        font_size: float = DEFAULT_FONT_SIZE,
-        include_underline: bool = True,
-        underline_width: float | None = None,
-        underline_buff: float = MED_SMALL_BUFF,
-        match_underline_width_to_text: bool = False,
-        depth: float | None = None,
-        **kwargs
-    ):
-        txt = Text(text, font=font, font_size=font_size, **kwargs)
-        txt.points.to_border(UP)
-
-        super().__init__(txt)
-        self.txt = txt
-
-        if include_underline:
-            if underline_width is None and not match_underline_width_to_text:
-                underline_width = Config.get.frame_width - 2
-
-            underline = Line(LEFT, RIGHT)
-            underline.points.next_to(txt, DOWN, buff=underline_buff)
-            if match_underline_width_to_text:
-                underline.points.set_width(txt.points.box.width)
-            else:
-                underline.points.set_width(underline_width)
-
-            self.add(underline)
-            self.underline = underline
-
-        self.depth.arrange(depth)
-
-
-class SourceDisplayer(Text):
-    '''
-    显示 ``obj`` 的源代码
-    '''
-    def __init__(
-        self,
-        obj,
-        font_size=12,
-        color=GREY,
-        **kwargs
-    ):
-        super().__init__(
-            inspect.getsource(obj),
-            font_size=font_size,
-            color=color,
-            **kwargs
-        )
-        self.points.to_border(UL)
+from __future__ import annotations
+
+import inspect
+import itertools as it
+import re
+from collections import defaultdict
+from enum import Enum
+from typing import Any, Callable, Concatenate, Iterable, Self
+
+import numpy as np
+
+from janim.components.points import Cmpt_Points
+from janim.constants import (DOWN, GREY, LEFT, MED_SMALL_BUFF, ORIGIN, RIGHT,
+                             UL, UP)
+from janim.exception import ColorNotFoundError
+from janim.items.geometry.line import Line
+from janim.items.points import Group, Points
+from janim.items.vitem import VItem
+from janim.logger import log
+from janim.typing import JAnimColor
+from janim.utils.config import Config
+from janim.utils.font import Font, get_fontpath_by_name
+from janim.utils.simple_functions import decode_utf8
+from janim.utils.space_ops import get_norm, normalize
+
+DEFAULT_FONT_SIZE = 24
+ORIG_FONT_SIZE = 48
+
+
+def _get_color_value(key: str) -> JAnimColor:
+    '''
+    根据 ``key`` 从 ``janim.constants.colors`` 得到颜色
+
+    如果 ``key`` 以 ``#`` 开头，则直接返回原值
+    '''
+    if key.startswith('#'):
+        return key
+
+    import janim.constants.colors as colors
+    if not hasattr(colors, key):
+        raise ColorNotFoundError(f'No built-in color named {key}')
+    return getattr(colors, key)
+
+
+type ActConverter = Callable[[str], Any]
+type ActCaller = Callable[Concatenate[TextChar, ...], Any]
+type Act = tuple[Iterable[ActConverter], ActCaller]
+type ActName = str
+
+type ActParams = Iterable[str]
+type ActParamsStack = list[ActParams]
+
+type ActAt = int
+type ActStart = tuple[ActName, ActParams]
+type ActEnd = str
+
+available_act_map: dict[ActName, list[Act]] = defaultdict(list)
+
+
+def _register_acts(names: list[ActName], *acts: Act) -> None:
+    '''
+    用于声明可用的富文本格式
+    '''
+    for name in names:
+        available_act_map[name].extend(acts)
+
+
+_register_acts(
+    ['color', 'c'],
+    ((_get_color_value,),           lambda char, color: char.color.set(color)),
+    ((float, float, float),         lambda char, r, g, b: char.color.set([r, g, b])),
+    ((float, float, float, float),  lambda char, r, g, b, a: char.color.set_rgbas([[r, g, b, a]]))
+)
+_register_acts(
+    ['stroke_color', 'sc'],
+    ((_get_color_value,),           lambda char, color: char.stroke.set(color)),
+    ((float, float, float),         lambda char, r, g, b: char.stroke.set([r, g, b])),
+    ((float, float, float, float),  lambda char, r, g, b, a: char.stroke.set_rgbas([[r, g, b, a]]))
+)
+_register_acts(
+    ['fill_color', 'fc'],
+    ((_get_color_value,),           lambda char, color: char.fill.set(color)),
+    ((float, float, float),         lambda char, r, g, b: char.fill.set([r, g, b])),
+    ((float, float, float, float),  lambda char, r, g, b, a: char.fill.set_rgbas([[r, g, b, a]]))
+)
+_register_acts(
+    ['alpha', 'a'],
+    ((float,), lambda char, a: char.color.set(alpha=a))
+)
+_register_acts(
+    ['stroke_alpha', 'sa'],
+    ((float,), lambda char, a: char.stroke.set(alpha=a))
+)
+_register_acts(
+    ['fill_alpha', 'fa'],
+    ((float,), lambda char, a: char.fill.set(alpha=a))
+)
+_register_acts(
+    ['stroke', 's'],
+    ((float,), lambda char, radius: char.radius.set(radius))
+)
+_register_acts(
+    ['font_scale', 'fs'],
+    ((float,), lambda char, factor: char.points.scale(factor, about_point=ORIGIN))
+)
+
+
+class TextChar(VItem):
+    '''
+    字符物件，作为 :class:`TextLine` 的子物件，在创建 :class:`TextLine` 时产生
+    '''
+    def __init__(
+        self,
+        char: str,
+        fonts: list[Font],
+        font_size: float,
+        fill_alpha=None,
+        **kwargs
+    ):
+        super().__init__(fill_alpha=fill_alpha, **kwargs)
+        self.char = char
+
+        unicode = decode_utf8(char)
+        font_render = self.get_font_for_render(unicode, fonts)
+
+        outline, advance = font_render.get_glyph_data(unicode)
+
+        font_scale_factor = font_size / ORIG_FONT_SIZE
+        frame_scale_factor = Config.get.pixel_to_frame_ratio / 32
+        scale_factor = font_scale_factor * frame_scale_factor
+
+        self.points.set(outline * scale_factor)
+
+        # 标记位置
+        self.mark = Points(
+            ORIGIN, RIGHT * font_scale_factor, UP * font_scale_factor,
+            [advance[0] * scale_factor, advance[1] * scale_factor, 0]
+        )
+        Cmpt_Points.apply_points_fn.connect(
+            self.points,
+            lambda func, about_point: self.mark.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
+        )
+
+    @staticmethod
+    def get_font_for_render(unicode: str, fonts: list[Font]) -> Font:
+        '''
+        从字体列表中找到支持显示 ``unicode`` 的字体，如果找不到只好选用第一个
+        '''
+        font_render = fonts[0]
+        for font in fonts:
+            idx = font.face.get_char_index(unicode)
+            if idx != 0:
+                font_render = font
+                break
+        return font_render
+
+    def get_mark_orig(self) -> np.ndarray:
+        return self.mark.points._points.data[0]
+
+    def get_mark_right(self) -> np.ndarray:
+        return self.mark.points._points.data[1]
+
+    def get_mark_up(self) -> np.ndarray:
+        return self.mark.points._points.data[2]
+
+    def get_mark_advance(self) -> np.ndarray:
+        return self.mark.points._points.data[3]
+
+    def get_advance_length(self) -> float:
+        return get_norm(self.get_mark_advance() - self.get_mark_orig())
+
+    def apply_act_list(self, act_params_map: dict[str, ActParamsStack]) -> None:
+        '''
+        应用富文本样式，由 :meth:`Text.apply_rich_text` 调用
+        '''
+        for name, params_stack in act_params_map.items():
+            params = params_stack[-1]
+            for converters, caller in available_act_map[name]:
+                if len(converters) == len(params):
+                    try:
+                        caller(
+                            self, *[
+                                converter(param)
+                                for converter, param in zip(converters, params)
+                            ]
+                        )
+                    except Exception:
+                        log.error(f'应用 {name} 时，{params} 与 {[cvt.__name__ for cvt in converters]} 不匹配')
+                        raise
+
+                    break
+            else:
+                txt = ','.join([
+                    '[' + ','.join([cvt.__name__ for cvt in act[0]]) + ']'
+                    for act in available_act_map[name]
+                ])
+                log.warning(f'应用 "{name}" 时，{params} 与 {txt} 没有匹配项')
+
+
+class TextLine(VItem, Group[TextChar]):
+    '''
+    单行文字物件，作为 :class:`Text` 的子物件，在创建 :class:`Text` 时产生s
+    '''
+    def __init__(
+        self,
+        text: str,
+        fonts: list[Font],
+        font_size: float,
+        char_kwargs={},
+        fill_alpha=None,
+        **kwargs
+    ):
+        self.text = text
+
+        super().__init__(
+            *[
+                TextChar(char, fonts, font_size, **char_kwargs)
+                for char in text
+            ],
+            fill_alpha=fill_alpha,
+            **kwargs
+        )
+
+        # 标记位置
+        self.mark = Points(ORIGIN, RIGHT, UP)
+        self.mark.points.scale(font_size / ORIG_FONT_SIZE, about_point=ORIGIN)
+        Cmpt_Points.apply_points_fn.connect(
+            self.points,
+            lambda func, about_point: self.mark.points.apply_points_fn(func,
+                                                                       about_point=about_point,
+                                                                       about_edge=None)
+        )
+
+    def get_mark_orig(self) -> np.ndarray:
+        return self.mark.points._points.data[0]
+
+    def get_mark_right(self) -> np.ndarray:
+        return self.mark.points._points.data[1]
+
+    def get_mark_up(self) -> np.ndarray:
+        return self.mark.points._points.data[2]
+
+    def arrange_in_line(self, buff: float = 0) -> Self:
+        '''
+        根据 ``advance`` 的标记信息排列该行
+        '''
+        if len(self.children) == 0:
+            return
+
+        pos = None
+
+        for i, char in enumerate(self):
+            if i != 0:
+                char.points.shift(pos - char.get_mark_orig())
+
+            orig = char.get_mark_orig()
+            advance = char.get_mark_advance()
+            pos = advance if buff == 0 else advance + buff * normalize(advance - orig)
+
+        return self
+
+
+class Text(VItem, Group[TextLine]):
+    '''
+    文字物件
+    '''
+    class Format(Enum):
+        PlainText = 0
+        RichText = 1
+
+    def __init__(
+        self,
+        text: str,
+        font: str | Iterable[str] = [],
+        font_size: float = DEFAULT_FONT_SIZE,
+        format: Format = Format.PlainText,
+        line_kwargs: dict = {},
+        stroke_alpha: float = 0,
+        fill_alpha: float = 1,
+        **kwargs
+    ) -> None:
+        # 获取字体
+        if isinstance(font, str):
+            font = [font]
+
+        cfg_font = Config.get.font
+        if isinstance(cfg_font, str):
+            font.append(cfg_font)
+        else:
+            font.extend(cfg_font)
+
+        fonts = [
+            Font.get(get_fontpath_by_name(name))
+            for name in font
+        ]
+
+        if format is not Text.Format.RichText:
+            self.text = text
+        else:
+            # 如果是 RichText，获取属性列表
+            self.text = ''
+            self.act_params_list: list[tuple[ActAt, ActStart | ActEnd]] = []
+            idx = 0
+            iter = re.finditer(r'(<+)(/?[^<]*?)>', text)
+            for match in iter:
+                match: re.Match
+                start, end = match.span()
+                left, mid = match.group(1, 2)
+
+                self.text += text[idx:start]
+                idx = end
+
+                left_cnt = len(left)
+                self.text += '<' * (left_cnt // 2)
+                if left_cnt % 2 == 0:
+                    self.text += mid + '>'
+                else:
+                    if mid.startswith('/'):
+                        self.act_params_list.append((len(self.text), mid[1:]))
+                    else:
+                        split = mid.split()
+                        self.act_params_list.append((len(self.text), (split[0], split[1:])))
+
+            self.text += text[idx:]
+
+        super().__init__(
+            *[
+                TextLine(line_text, fonts=fonts, font_size=font_size, **line_kwargs)
+                for line_text in self.text.split('\n')
+            ],
+            stroke_alpha=stroke_alpha,
+            fill_alpha=fill_alpha,
+            **kwargs
+        )
+
+        if format is Text.Format.RichText:
+            self.apply_rich_text()
+        for line in self.children:
+            line.arrange_in_line()
+        self.arrange_in_lines()
+        self.astype(Points).points.to_center()
+
+    def is_null(self) -> bool:
+        return True
+
+    def idx_to_row_col(self, idx: int) -> tuple[int, int]:
+        '''
+        由字符索引得到 行数、列数 索引
+        '''
+        for i, line in enumerate(self):
+            if idx < len(line):
+                return i, idx
+            idx -= len(line)
+        return len(self) - 1, idx
+
+    def select_parts(self, pattern):
+        '''
+        根据 ``pattern`` 获得文字中的部分
+        '''
+        total_text: str = ''.join([line.text for line in self])
+        parts = []
+        for mch in re.finditer(pattern, total_text):
+            l_row, l_col = self.idx_to_row_col(mch.start())
+            r_row, r_col = self.idx_to_row_col(mch.end())
+            if l_row == r_row:
+                parts.append(self[l_row][l_col:r_col])
+            else:
+                parts.append(
+                    Group(*it.chain(
+                        self[l_row][l_col:],
+                        *self[l_row + 1: r_row],
+                        self[r_row][:r_col]
+                    ))
+                )
+        return Group(*parts)
+
+    def arrange_in_lines(self, buff: float = 0, base_buff: float = 0.85) -> Self:
+        '''
+        - ``buff``: 每行之间的额外间距
+        - ``base_buff``: 每行之间的基本间距，默认值 ``0.85`` 用于将两行上下排列，如果是 ``0`` 则会让两行完全重合，大部分时候不需要传入该值
+        '''
+        if len(self.children) == 0:
+            return
+
+        pos = self.children[0].get_mark_orig()
+        for line in self.children[1:]:
+            vert = line.get_mark_orig() - line.get_mark_up()
+            target = pos + base_buff * vert + buff * normalize(vert)
+            line.points.shift(
+                target - line.get_mark_orig()
+            )
+            pos = line.get_mark_orig()
+
+        return self
+
+    # TODO: word_wrap
+    # 使用 TypstDoc 可以轻松做到
+    # 我感觉可以不用给 Text 实现这功能了
+
+    def apply_rich_text(self) -> None:
+        '''
+        应用富文本效果
+        '''
+        text_at = 0
+        act_idx = 0
+        act_params_map: defaultdict[str, ActParamsStack] = defaultdict(list)
+        for line in self.children:
+            for char in line.children:
+                while act_idx < len(self.act_params_list):
+                    next_act_at, next_act = self.act_params_list[act_idx]
+                    if text_at < next_act_at:
+                        break
+
+                    if isinstance(next_act, str):   # ActEnd
+                        stack = act_params_map[next_act]
+                        stack.pop()
+                        if not stack:
+                            del act_params_map[next_act]
+                    else:   # ActStart
+                        name, params = next_act
+                        act_params_map[name].append(params)
+
+                    act_idx += 1
+
+                char.apply_act_list(act_params_map)
+                text_at += 1
+
+            text_at += 1
+
+
+class Title(Group):
+    '''
+    标题
+
+    - ``include_underline=True`` 会添加下划线（默认添加）
+    - ``underline_width`` 下划线的长度（默认屏幕宽 - 2 个单位）
+    - ``match_underline_width_to_text=True`` 时将下划线的长度和文字匹配（默认为 ``False``）
+    '''
+    def __init__(
+        self,
+        text: str,
+        font: str | Iterable[str] = [],
+        font_size: float = DEFAULT_FONT_SIZE,
+        include_underline: bool = True,
+        underline_width: float | None = None,
+        underline_buff: float = MED_SMALL_BUFF,
+        match_underline_width_to_text: bool = False,
+        depth: float | None = None,
+        **kwargs
+    ):
+        txt = Text(text, font=font, font_size=font_size, **kwargs)
+        txt.points.to_border(UP)
+
+        super().__init__(txt)
+        self.txt = txt
+
+        if include_underline:
+            if underline_width is None and not match_underline_width_to_text:
+                underline_width = Config.get.frame_width - 2
+
+            underline = Line(LEFT, RIGHT)
+            underline.points.next_to(txt, DOWN, buff=underline_buff)
+            if match_underline_width_to_text:
+                underline.points.set_width(txt.points.box.width)
+            else:
+                underline.points.set_width(underline_width)
+
+            self.add(underline)
+            self.underline = underline
+
+        self.depth.arrange(depth)
+
+
+class SourceDisplayer(Text):
+    '''
+    显示 ``obj`` 的源代码
+    '''
+    def __init__(
+        self,
+        obj,
+        font_size=12,
+        color=GREY,
+        **kwargs
+    ):
+        super().__init__(
+            inspect.getsource(obj),
+            font_size=font_size,
+            color=color,
+            **kwargs
+        )
+        self.points.to_border(UL)
```

### Comparing `janim-1.0.4/janim/render/impl.py` & `janim-1.1.0/janim/render/impl.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-
-from typing import TYPE_CHECKING
-
-import moderngl as mgl
-import numpy as np
-
-from janim.render.base import Renderer, get_program
-from janim.render.texture import get_texture_from_img
-from janim.utils.iterables import resize_with_interpolation
-
-if TYPE_CHECKING:
-    from janim.items.image_item import ImageItem
-    from janim.items.points import DotCloud
-    from janim.items.vitem import VItem
-
-
-class DotCloudRenderer(Renderer):
-    def init(self) -> None:
-        self.prog = get_program('render/shaders/dotcloud')
-
-        self.ctx = self.data_ctx.get().ctx
-        self.vbo_points = self.ctx.buffer(reserve=1)
-        self.vbo_color = self.ctx.buffer(reserve=1)
-        self.vbo_radius = self.ctx.buffer(reserve=1)
-
-        self.vao = self.ctx.vertex_array(self.prog, [
-            (self.vbo_points, '3f', 'in_point'),
-            (self.vbo_color, '4f', 'in_color'),
-            (self.vbo_radius, '1f', 'in_radius')
-        ])
-
-        self.prev_points = np.array([])
-        self.prev_color = np.array([])
-        self.prev_radius = np.array([])
-
-    def render(self, item: 'DotCloud') -> None:
-        new_color = item.color._rgbas.data
-        new_radius = item.radius._radii.data
-        new_points = item.points._points.data
-
-        if id(new_color) != id(self.prev_color) or len(new_points) != len(self.prev_points):
-            color = resize_with_interpolation(new_color, len(new_points))
-            bytes = color.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_color.size:
-                self.vbo_color.orphan(len(bytes))
-
-            self.vbo_color.write(bytes)
-            self.prev_color = new_color
-
-        if id(new_radius) != id(self.prev_radius) or len(new_points) != len(self.prev_points):
-            radius = resize_with_interpolation(new_radius, len(new_points))
-            bytes = radius.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_radius.size:
-                self.vbo_radius.orphan(len(bytes))
-
-            self.vbo_radius.write(bytes)
-            self.prev_radius = new_radius
-
-        if id(new_points) != id(self.prev_points):
-            bytes = new_points.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_points.size:
-                self.vbo_points.orphan(len(bytes))
-
-            self.vbo_points.write(bytes)
-            self.prev_points = new_points
-
-        self.vao.render(mgl.POINTS, vertices=len(self.prev_points))
-
-
-class VItemRenderer(Renderer):
-    def init(self) -> None:
-        self.prog = get_program('render/shaders/vitem')
-
-        self.ctx = self.data_ctx.get().ctx
-        self.vbo_coord = self.ctx.buffer(reserve=4 * 2 * 4)
-        self.vbo_mapped_points = self.ctx.buffer(reserve=1)
-        self.vbo_radius = self.ctx.buffer(reserve=1)
-        self.vbo_stroke_color = self.ctx.buffer(reserve=1)
-        self.vbo_fill_color = self.ctx.buffer(reserve=1)
-
-        self.vao = self.ctx.vertex_array(self.prog, self.vbo_coord, 'in_coord')
-
-        self.prev_camera_info = None
-
-        self.prev_points = np.array([])
-        self.prev_radius = np.array([])
-        self.prev_stroke = np.array([])
-        self.prev_fill = np.array([])
-
-    def render(self, item: 'VItem') -> None:
-        if item.points.curves_count() == 0:
-            return
-        render_data = self.data_ctx.get()
-
-        new_camera_info = render_data.camera_info
-
-        new_points = item.points._points.data
-        new_radius = item.radius._radii.data
-        new_stroke = item.stroke._rgbas.data
-        new_fill = item.fill._rgbas.data
-
-        is_camera_changed = id(new_camera_info) != id(self.prev_camera_info)
-
-        if id(new_radius) != id(self.prev_radius) or id(new_points) != id(self.prev_points) or is_camera_changed:
-            clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
-            clip_box *= render_data.camera_info.frame_radius
-
-            buff = new_radius.max() + render_data.anti_alias_radius
-            clip_min = np.min(clip_box, axis=0) - buff
-            clip_max = np.max(clip_box, axis=0) + buff
-            clip_box = np.array([
-                clip_min,
-                [clip_min[0], clip_max[1]],
-                [clip_max[0], clip_min[1]],
-                clip_max
-            ]) / render_data.camera_info.frame_radius
-            clip_box = np.clip(clip_box, -1, 1)
-
-            bytes = clip_box.astype('f4').tobytes()
-            assert len(bytes) == self.vbo_coord.size
-            self.vbo_coord.write(bytes)
-
-        if id(new_radius) != id(self.prev_radius) or len(new_points) != len(self.prev_points):
-            radius = resize_with_interpolation(new_radius, (len(new_points) + 1) // 2)
-            bytes = radius.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_radius.size:
-                self.vbo_radius.orphan(len(bytes))
-
-            self.vbo_radius.write(bytes)
-            self.prev_radius = new_radius
-
-        if id(new_stroke) != id(self.prev_stroke) or len(new_points) != len(self.prev_points):
-            stroke = resize_with_interpolation(new_stroke, (len(new_points) + 1) // 2)
-            bytes = stroke.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_stroke_color.size:
-                self.vbo_stroke_color.orphan(len(bytes))
-
-            self.vbo_stroke_color.write(bytes)
-            self.prev_stroke = new_stroke
-
-        if id(new_fill) != id(self.prev_fill) or len(new_points) != len(self.prev_points):
-            fill = resize_with_interpolation(new_fill, (len(new_points) + 1) // 2)
-            bytes = fill.astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_fill_color.size:
-                self.vbo_fill_color.orphan(len(bytes))
-
-            self.vbo_fill_color.write(bytes)
-            self.prev_fill = new_fill
-
-        if id(new_points) != id(self.prev_points) or is_camera_changed:
-            mapped = render_data.camera_info.map_points(new_points)
-            mapped *= render_data.camera_info.frame_radius
-
-            bytes = np.hstack([
-                mapped,
-                item.points.get_closepath_flags()[:, np.newaxis],
-                np.zeros((len(mapped), 1))
-            ]).astype('f4').tobytes()
-
-            if len(bytes) != self.vbo_mapped_points.size:
-                self.vbo_mapped_points.orphan(len(bytes))
-
-            self.vbo_mapped_points.write(bytes)
-            self.prev_camera_info = new_camera_info
-            self.prev_points = new_points
-
-        self.vbo_mapped_points.bind_to_storage_buffer(0)
-        self.vbo_radius.bind_to_storage_buffer(1)
-        self.vbo_stroke_color.bind_to_storage_buffer(2)
-        self.vbo_fill_color.bind_to_storage_buffer(3)
-        self.vao.render(mgl.TRIANGLE_STRIP)
-
-
-class ImageItemRenderer(Renderer):
-    def init(self) -> None:
-        self.prog = get_program('render/shaders/image')
-
-        self.ctx = self.data_ctx.get().ctx
-        self.vbo_points = self.ctx.buffer(reserve=4 * 3 * 4)
-        self.vbo_color = self.ctx.buffer(reserve=4 * 4 * 4)
-        self.vbo_texcoords = self.ctx.buffer(
-            data=np.array([
-                [0.0, 0.0],     # 左上
-                [0.0, 1.0],     # 左下
-                [1.0, 0.0],     # 右上
-                [1.0, 1.0]      # 右下
-            ]).astype('f4').tobytes()
-        )
-
-        self.vao = self.ctx.vertex_array(self.prog, [
-            (self.vbo_points, '3f', 'in_point'),
-            (self.vbo_color, '4f', 'in_color'),
-            (self.vbo_texcoords, '2f', 'in_texcoord')
-        ])
-
-        self.prev_points = np.array([])
-        self.prev_color = np.array([])
-        self.prev_img = None
-
-    def render(self, item: 'ImageItem') -> None:
-        new_color = item.color._rgbas.data
-        new_points = item.points._points.data
-
-        if id(new_color) != id(self.prev_color):
-            color = resize_with_interpolation(new_color, 4)
-            bytes = color.astype('f4').tobytes()
-
-            assert len(bytes) == self.vbo_color.size
-
-            self.vbo_color.write(bytes)
-            self.prev_color = new_color
-
-        if id(new_points) != id(self.prev_points):
-            bytes = new_points.astype('f4').tobytes()
-
-            assert len(bytes) == self.vbo_points.size
-
-            self.vbo_points.write(bytes)
-            self.prev_points = new_points
-
-        if self.prev_img is None or item.image.img is not self.prev_img:
-            self.texture = get_texture_from_img(item.image.get())
-            self.texture.build_mipmaps()
-            self.prev_img = item.image.img
-
-        self.prog['image'] = 0
-        self.texture.filter = item.image.get_filter()
-        self.texture.use(0)
-        self.vao.render(mgl.TRIANGLE_STRIP)
+
+from typing import TYPE_CHECKING
+
+import moderngl as mgl
+import numpy as np
+
+from janim.render.base import Renderer, get_program
+from janim.render.texture import get_texture_from_img
+from janim.utils.iterables import resize_with_interpolation
+
+if TYPE_CHECKING:
+    from janim.items.image_item import ImageItem
+    from janim.items.points import DotCloud
+    from janim.items.vitem import VItem
+
+
+class DotCloudRenderer(Renderer):
+    def init(self) -> None:
+        self.prog = get_program('render/shaders/dotcloud')
+
+        self.ctx = self.data_ctx.get().ctx
+        self.vbo_points = self.ctx.buffer(reserve=1)
+        self.vbo_color = self.ctx.buffer(reserve=1)
+        self.vbo_radius = self.ctx.buffer(reserve=1)
+
+        self.vao = self.ctx.vertex_array(self.prog, [
+            (self.vbo_points, '3f', 'in_point'),
+            (self.vbo_color, '4f', 'in_color'),
+            (self.vbo_radius, '1f', 'in_radius')
+        ])
+
+        self.prev_points = np.array([])
+        self.prev_color = np.array([])
+        self.prev_radius = np.array([])
+
+    def render(self, item: 'DotCloud') -> None:
+        new_color = item.color._rgbas.data
+        new_radius = item.radius._radii.data
+        new_points = item.points._points.data
+
+        if id(new_color) != id(self.prev_color) or len(new_points) != len(self.prev_points):
+            color = resize_with_interpolation(new_color, len(new_points))
+            bytes = color.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_color.size:
+                self.vbo_color.orphan(len(bytes))
+
+            self.vbo_color.write(bytes)
+            self.prev_color = new_color
+
+        if id(new_radius) != id(self.prev_radius) or len(new_points) != len(self.prev_points):
+            radius = resize_with_interpolation(new_radius, len(new_points))
+            bytes = radius.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_radius.size:
+                self.vbo_radius.orphan(len(bytes))
+
+            self.vbo_radius.write(bytes)
+            self.prev_radius = new_radius
+
+        if id(new_points) != id(self.prev_points):
+            bytes = new_points.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_points.size:
+                self.vbo_points.orphan(len(bytes))
+
+            self.vbo_points.write(bytes)
+            self.prev_points = new_points
+
+        self.vao.render(mgl.POINTS, vertices=len(self.prev_points))
+
+
+class VItemRenderer(Renderer):
+    def init(self) -> None:
+        self.prog = get_program('render/shaders/vitem')
+
+        self.ctx = self.data_ctx.get().ctx
+        self.vbo_coord = self.ctx.buffer(reserve=4 * 2 * 4)
+        self.vbo_mapped_points = self.ctx.buffer(reserve=1)
+        self.vbo_radius = self.ctx.buffer(reserve=1)
+        self.vbo_stroke_color = self.ctx.buffer(reserve=1)
+        self.vbo_fill_color = self.ctx.buffer(reserve=1)
+
+        self.vao = self.ctx.vertex_array(self.prog, self.vbo_coord, 'in_coord')
+
+        self.prev_camera_info = None
+
+        self.prev_points = np.array([])
+        self.prev_radius = np.array([])
+        self.prev_stroke = np.array([])
+        self.prev_fill = np.array([])
+
+    def render(self, item: 'VItem') -> None:
+        if item.points.curves_count() == 0:
+            return
+        render_data = self.data_ctx.get()
+
+        new_camera_info = render_data.camera_info
+
+        new_points = item.points._points.data
+        new_radius = item.radius._radii.data
+        new_stroke = item.stroke._rgbas.data
+        new_fill = item.fill._rgbas.data
+
+        is_camera_changed = id(new_camera_info) != id(self.prev_camera_info)
+
+        if id(new_radius) != id(self.prev_radius) or id(new_points) != id(self.prev_points) or is_camera_changed:
+            clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
+            clip_box *= render_data.camera_info.frame_radius
+
+            buff = new_radius.max() + render_data.anti_alias_radius
+            clip_min = np.min(clip_box, axis=0) - buff
+            clip_max = np.max(clip_box, axis=0) + buff
+            clip_box = np.array([
+                clip_min,
+                [clip_min[0], clip_max[1]],
+                [clip_max[0], clip_min[1]],
+                clip_max
+            ]) / render_data.camera_info.frame_radius
+            clip_box = np.clip(clip_box, -1, 1)
+
+            bytes = clip_box.astype('f4').tobytes()
+            assert len(bytes) == self.vbo_coord.size
+            self.vbo_coord.write(bytes)
+
+        if id(new_radius) != id(self.prev_radius) or len(new_points) != len(self.prev_points):
+            radius = resize_with_interpolation(new_radius, (len(new_points) + 1) // 2)
+            bytes = radius.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_radius.size:
+                self.vbo_radius.orphan(len(bytes))
+
+            self.vbo_radius.write(bytes)
+            self.prev_radius = new_radius
+
+        if id(new_stroke) != id(self.prev_stroke) or len(new_points) != len(self.prev_points):
+            stroke = resize_with_interpolation(new_stroke, (len(new_points) + 1) // 2)
+            bytes = stroke.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_stroke_color.size:
+                self.vbo_stroke_color.orphan(len(bytes))
+
+            self.vbo_stroke_color.write(bytes)
+            self.prev_stroke = new_stroke
+
+        if id(new_fill) != id(self.prev_fill) or len(new_points) != len(self.prev_points):
+            fill = resize_with_interpolation(new_fill, (len(new_points) + 1) // 2)
+            bytes = fill.astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_fill_color.size:
+                self.vbo_fill_color.orphan(len(bytes))
+
+            self.vbo_fill_color.write(bytes)
+            self.prev_fill = new_fill
+
+        if id(new_points) != id(self.prev_points) or is_camera_changed:
+            mapped = render_data.camera_info.map_points(new_points)
+            mapped *= render_data.camera_info.frame_radius
+
+            bytes = np.hstack([
+                mapped,
+                item.points.get_closepath_flags()[:, np.newaxis],
+                np.zeros((len(mapped), 1))
+            ]).astype('f4').tobytes()
+
+            if len(bytes) != self.vbo_mapped_points.size:
+                self.vbo_mapped_points.orphan(len(bytes))
+
+            self.vbo_mapped_points.write(bytes)
+            self.prev_camera_info = new_camera_info
+            self.prev_points = new_points
+
+        self.vbo_mapped_points.bind_to_storage_buffer(0)
+        self.vbo_radius.bind_to_storage_buffer(1)
+        self.vbo_stroke_color.bind_to_storage_buffer(2)
+        self.vbo_fill_color.bind_to_storage_buffer(3)
+        self.vao.render(mgl.TRIANGLE_STRIP)
+
+
+class ImageItemRenderer(Renderer):
+    def init(self) -> None:
+        self.prog = get_program('render/shaders/image')
+
+        self.ctx = self.data_ctx.get().ctx
+        self.vbo_points = self.ctx.buffer(reserve=4 * 3 * 4)
+        self.vbo_color = self.ctx.buffer(reserve=4 * 4 * 4)
+        self.vbo_texcoords = self.ctx.buffer(
+            data=np.array([
+                [0.0, 0.0],     # 左上
+                [0.0, 1.0],     # 左下
+                [1.0, 0.0],     # 右上
+                [1.0, 1.0]      # 右下
+            ]).astype('f4').tobytes()
+        )
+
+        self.vao = self.ctx.vertex_array(self.prog, [
+            (self.vbo_points, '3f', 'in_point'),
+            (self.vbo_color, '4f', 'in_color'),
+            (self.vbo_texcoords, '2f', 'in_texcoord')
+        ])
+
+        self.prev_points = np.array([])
+        self.prev_color = np.array([])
+        self.prev_img = None
+
+    def render(self, item: 'ImageItem') -> None:
+        new_color = item.color._rgbas.data
+        new_points = item.points._points.data
+
+        if id(new_color) != id(self.prev_color):
+            color = resize_with_interpolation(new_color, 4)
+            bytes = color.astype('f4').tobytes()
+
+            assert len(bytes) == self.vbo_color.size
+
+            self.vbo_color.write(bytes)
+            self.prev_color = new_color
+
+        if id(new_points) != id(self.prev_points):
+            bytes = new_points.astype('f4').tobytes()
+
+            assert len(bytes) == self.vbo_points.size
+
+            self.vbo_points.write(bytes)
+            self.prev_points = new_points
+
+        if self.prev_img is None or item.image.img is not self.prev_img:
+            self.texture = get_texture_from_img(item.image.get())
+            self.texture.build_mipmaps()
+            self.prev_img = item.image.img
+
+        self.prog['image'] = 0
+        self.texture.filter = item.image.get_filter()
+        self.texture.use(0)
+        self.vao.render(mgl.TRIANGLE_STRIP)
```

### Comparing `janim-1.0.4/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.1.0/janim/render/shaders/dotcloud.geom.glsl`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#version 330 core
-layout (points) in;
-layout (triangle_strip, max_vertices = 4) out;
-
-in vec4 v_pos[1];
-in vec4 v_color[1];
-in float v_radius[1];
-
-out vec2 g_center;
-out vec4 g_color;
-out float g_radius;
-out vec2 g_point;
-
-uniform mat4 JA_PROJ_MATRIX;
-uniform vec2 JA_FRAME_RADIUS;
-uniform float JA_ANTI_ALIAS_RADIUS;
-
-vec4 normalize_w(vec4 vect)
-{
-    return vect / vect.w;
-}
-
-void main()
-{
-    vec4 corners[4];
-    for (int i = 0; i < 4; i++) {
-        vec2 direction = vec2(
-            2 * (i % 2) - 1,
-            2 * (i / 2) - 1
-        );
-        corners[i] = v_pos[0];
-        corners[i].xy += v_radius[0] * direction;
-        corners[i] = normalize_w(JA_PROJ_MATRIX * corners[i]);
-        corners[i].xy *= JA_FRAME_RADIUS;
-        corners[i].xy += JA_ANTI_ALIAS_RADIUS * direction;
-    }
-
-    g_center = normalize_w(JA_PROJ_MATRIX * v_pos[0]).xy * JA_FRAME_RADIUS;
-    g_color = v_color[0];
-    g_radius = (corners[1].x - corners[0].x) / 2.0 - JA_ANTI_ALIAS_RADIUS;
-
-    for (int i = 0; i < 4; i++) {
-        g_point = corners[i].xy;
-        gl_Position = corners[i];
-        gl_Position.xy /= JA_FRAME_RADIUS;
-        gl_Position.z *= 0.1;
-        EmitVertex();
-    }
-    EndPrimitive();
-}
+#version 330 core
+layout (points) in;
+layout (triangle_strip, max_vertices = 4) out;
+
+in vec4 v_pos[1];
+in vec4 v_color[1];
+in float v_radius[1];
+
+out vec2 g_center;
+out vec4 g_color;
+out float g_radius;
+out vec2 g_point;
+
+uniform mat4 JA_PROJ_MATRIX;
+uniform vec2 JA_FRAME_RADIUS;
+uniform float JA_ANTI_ALIAS_RADIUS;
+
+vec4 normalize_w(vec4 vect)
+{
+    return vect / vect.w;
+}
+
+void main()
+{
+    vec4 corners[4];
+    for (int i = 0; i < 4; i++) {
+        vec2 direction = vec2(
+            2 * (i % 2) - 1,
+            2 * (i / 2) - 1
+        );
+        corners[i] = v_pos[0];
+        corners[i].xy += v_radius[0] * direction;
+        corners[i] = normalize_w(JA_PROJ_MATRIX * corners[i]);
+        corners[i].xy *= JA_FRAME_RADIUS;
+        corners[i].xy += JA_ANTI_ALIAS_RADIUS * direction;
+    }
+
+    g_center = normalize_w(JA_PROJ_MATRIX * v_pos[0]).xy * JA_FRAME_RADIUS;
+    g_color = v_color[0];
+    g_radius = (corners[1].x - corners[0].x) / 2.0 - JA_ANTI_ALIAS_RADIUS;
+
+    for (int i = 0; i < 4; i++) {
+        g_point = corners[i].xy;
+        gl_Position = corners[i];
+        gl_Position.xy /= JA_FRAME_RADIUS;
+        gl_Position.z *= 0.1;
+        EmitVertex();
+    }
+    EndPrimitive();
+}
```

### Comparing `janim-1.0.4/janim/render/shaders/vitem.frag.glsl` & `janim-1.1.0/janim/render/shaders/vitem.frag.glsl`

 * *Files 22% similar despite different names*

```diff
@@ -1,254 +1,255 @@
-#version 430 core
-
-in vec2 v_coord;
-
-out vec4 f_color;
-
-uniform float JA_ANTI_ALIAS_RADIUS;
-
-const float INFINITY = uintBitsToFloat(0x7F800000);
-
-layout(std140, binding = 0) buffer MappedPoints
-{
-    vec4 points[];  // vec4(x, y, isclosed, 0)
-};
-layout(std140, binding = 1) buffer Radii
-{
-    vec4 radii[];   // radii[idx / 4][idx % 4]
-};
-layout(std140, binding = 2) buffer Colors
-{
-    vec4 colors[];
-};
-layout(std140, binding = 3) buffer Fills
-{
-    vec4 fills[];
-};
-
-vec2 get_point(int idx) {
-    return points[idx].xy;
-}
-
-bool get_isclosed(int idx) {
-    return bool(points[idx].z);
-}
-
-float get_radius(int idx) {
-    return radii[idx / 4][idx % 4];
-}
-
-vec4 blend_color(vec4 fore, vec4 back) {
-    float a = fore.a + back.a * (1 - fore.a);
-    return clamp(
-        vec4(
-            (fore.rgb * fore.a + back.rgb * back.a * (1 - fore.a)) / a,
-            a
-        ),
-        0.0, 1.0
-    );
-}
-
-float cross2d(vec2 a, vec2 b) {
-    return a.x * b.y - a.y * b.x;
-}
-
-float sign_bezier(vec2 A, vec2 B, vec2 C, vec2 p)
-{
-    vec2 a = C - A, b = B - A, c = p - A;
-    vec2 bary = vec2(
-        c.x * b.y - b.x * c.y,
-        a.x * c.y - c.x * a.y
-    ) / (a.x * b.y - b.x * a.y);
-    vec2 d = vec2(bary.y * 0.5, 0.0) + 1.0 - bary.x - bary.y;
-
-    float sign_bezierInside = d.x > d.y ? sign(d.x * d.x - d.y) : 1.0;
-
-    bvec3 cond = bvec3( p.y >= A.y,
-                        p.y <  C.y,
-                        a.x * c.y > a.y * c.x );
-    float signLineLeft = all(cond) || all(not(cond)) ? -1.0 : 1.0;
-
-    return sign_bezierInside * signLineLeft;
-}
-
-vec3 solve_cubic(float a, float b, float c)
-{
-    float p = b - a * a / 3.0, p3 = p * p * p;
-    float q = a * (2.0 * a * a - 9.0 * b) / 27.0 + c;
-    float d = q * q + 4.0 * p3 / 27.0;
-    float offset = -a / 3.0;
-    if(d >= 0.0) {
-        float z = sqrt(d);
-        vec2 x = (vec2(z, -z) - q) / 2.0;
-        vec2 uv = sign(x) * pow(abs(x), vec2(1.0 / 3.0));
-        return vec3(offset + uv.x + uv.y);
-    }
-    float v = acos(-sqrt(-27.0 / p3) * q / 2.0) / 3.0;
-    float m = cos(v), n = sin(v) * 1.732050808;
-    return vec3(m + m, -n - m, n - m) * sqrt(-p / 3.0) + offset;
-}
-
-float distance_bezier(vec2 A, vec2 B, vec2 C, vec2 p)
-{
-    B = mix(B + vec2(1e-4), B, abs(sign(B * 2.0 - A - C)));
-    vec2 a = B - A, b = A - B * 2.0 + C, c = a * 2.0, d = A - p;
-    vec3 k = vec3(3. * dot(a, b),2. * dot(a, a) + dot(d, b),dot(d, a)) / dot(b, b);
-    vec3 t = clamp(solve_cubic(k.x, k.y, k.z), 0.0, 1.0);
-    vec2 pos = A + (c + b * t.x) * t.x;
-    float dis = length(pos - p);
-    pos = A + (c + b * t.y) * t.y;
-    dis = min(dis, length(pos - p));
-    pos = A + (c + b * t.z) * t.z;
-    dis = min(dis, length(pos - p));
-    return dis;
-}
-
-const int lim = (points.length() - 1) / 2 * 2;
-
-void get_subpath_attr(
-    int start_idx,
-    out int end_idx,
-    out int idx,
-    out float d,
-    out float sgn
-) {
-    end_idx = lim;
-    bool is_closed = get_isclosed(start_idx);
-
-    d = INFINITY;
-    sgn = 1.0;
-    for (int i = start_idx; i < lim; i += 2) {
-        vec2 B = get_point(i + 1);
-        if (isnan(B.x)) {
-            end_idx = i;
-            break;
-        }
-        vec2 A = get_point(i), C = get_point(i + 2);
-        if (A == B && B == C)
-            continue;
-
-        vec2 v1 = normalize(B - A);
-        vec2 v2 = normalize(C - B);
-        // REFACTOR: 使用更好的判断可近似为直线的方法
-        if (abs(cross2d(v1, v2)) < 1e-3 && dot(v1, v2) > 0.0) {
-            vec2 e = C - A;
-            vec2 w = v_coord - A;
-            vec2 b = w - e * clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
-            float dist = length(b);
-            if (dist < d) {
-                d = dist;
-                idx = i;
-            }
-
-            if (is_closed) {
-                bvec3 cond = bvec3( v_coord.y >= A.y,
-                                    v_coord.y  < C.y,
-                                    e.x * w.y > e.y * w.x );
-                if(all(cond) || all(not(cond))) sgn = -sgn;
-            }
-        } else {
-            float dist = distance_bezier(A, B, C, v_coord);
-            if (dist < d) {
-                d = dist;
-                idx = i;
-            }
-
-            if (is_closed) {
-                sgn *= sign_bezier(A, B, C, v_coord);
-            }
-        }
-    }
-}
-
-// #define CONTROL_POINTS
-// #define POLYGON_LINES
-// #define SDF_PLANE
-
-void main()
-{
-    float d;
-
-    #ifdef CONTROL_POINTS
-
-    d = distance(v_coord, get_point(0));
-    for (int i = 1; i < points.length(); i++) {
-        d = min(d, distance(v_coord, get_point(i)));
-    }
-    if (d < 0.06) {
-        f_color = vec4(1.0 - smoothstep(0.048, 0.052, d));
-        return;
-    }
-
-    #endif
-
-    int idx;
-    d = INFINITY;
-    float sgn = 1.0;
-
-    int start_idx = 0;
-    float sp_d;
-    float sp_sgn;
-
-    while (true) {
-        get_subpath_attr(start_idx, start_idx, idx, sp_d, sp_sgn);
-        d = min(d, sp_d);
-        sgn *= sp_sgn;
-
-        if (start_idx >= lim)
-            break;
-        start_idx += 2;
-    }
-    int anchor_idx = idx / 2;
-    float sgn_d = sgn * d;
-
-    vec2 e = get_point(idx + 2) - get_point(idx);
-    vec2 w = v_coord - get_point(idx);
-    float ratio = clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
-
-    float radius = mix(get_radius(anchor_idx), get_radius(anchor_idx + 1), ratio);
-
-    vec4 fill_color = get_isclosed(idx) ? mix(fills[anchor_idx], fills[anchor_idx + 1], ratio) : vec4(0.0);
-    fill_color.a *= smoothstep(1, -1, (sgn_d) / JA_ANTI_ALIAS_RADIUS);
-
-    vec4 stroke_color = mix(colors[anchor_idx], colors[anchor_idx + 1], ratio);
-    stroke_color.a *= smoothstep(1, -1, (d - radius) / JA_ANTI_ALIAS_RADIUS);
-
-    f_color = blend_color(stroke_color, fill_color);
-
-    #if !defined(POLYGON_LINES) && !defined(SDF_PLANE)
-    if (f_color.a == 0.0)
-        discard;
-    #endif
-
-    #ifdef SDF_PLANE
-
-    vec4 df_color = vec4(1.0) - sgn * vec4(0.1, 0.4, 0.7, 0.0);
-    df_color *= 0.8 + 0.2 * cos(140. * d / 3.0);
-    df_color = mix(df_color, vec4(1.0), 1.0 - smoothstep(0.0, 0.02, abs(d)));
-    df_color.a = 0.5;
-    f_color = blend_color(df_color, f_color);
-
-    #endif
-
-    #ifdef POLYGON_LINES
-
-    const int num = points.length();
-    d = dot(v_coord - get_point(0), v_coord - get_point(0));
-    for(int i = 1, j = 0; i < num; j = i, i++)
-    {
-        if (get_point(j) == get_point(i)) {
-            i++;
-            continue;
-        }
-        // distance
-        vec2 e = get_point(j) - get_point(i);
-        vec2 w = v_coord - get_point(i);
-        vec2 b = w - e * clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
-        d = min(d, dot(b, b));
-    }
-    float line_ratio = smoothstep(1.15, 0.85, sqrt(d) / 0.02);
-    f_color.g = max(line_ratio, f_color.g);
-    f_color.a = max(line_ratio, f_color.a);
-
-    #endif
+#version 430 core
+
+in vec2 v_coord;
+
+out vec4 f_color;
+
+uniform float JA_ANTI_ALIAS_RADIUS;
+
+const float INFINITY = uintBitsToFloat(0x7F800000);
+
+layout(std140, binding = 0) buffer MappedPoints
+{
+    vec4 points[];  // vec4(x, y, isclosed, 0)
+};
+layout(std140, binding = 1) buffer Radii
+{
+    vec4 radii[];   // radii[idx / 4][idx % 4]
+};
+layout(std140, binding = 2) buffer Colors
+{
+    vec4 colors[];
+};
+layout(std140, binding = 3) buffer Fills
+{
+    vec4 fills[];
+};
+
+vec2 get_point(int idx) {
+    return points[idx].xy;
+}
+
+bool get_isclosed(int idx) {
+    return bool(points[idx].z);
+}
+
+float get_radius(int idx) {
+    return radii[idx / 4][idx % 4];
+}
+
+vec4 blend_color(vec4 fore, vec4 back) {
+    float a = fore.a + back.a * (1 - fore.a);
+    return clamp(
+        vec4(
+            (fore.rgb * fore.a + back.rgb * back.a * (1 - fore.a)) / a,
+            a
+        ),
+        0.0, 1.0
+    );
+}
+
+float cross2d(vec2 a, vec2 b) {
+    return a.x * b.y - a.y * b.x;
+}
+
+float sign_bezier(vec2 A, vec2 B, vec2 C, vec2 p)
+{
+    vec2 a = C - A, b = B - A, c = p - A;
+    vec2 bary = vec2(
+        c.x * b.y - b.x * c.y,
+        a.x * c.y - c.x * a.y
+    ) / (a.x * b.y - b.x * a.y);
+    vec2 d = vec2(bary.y * 0.5, 0.0) + 1.0 - bary.x - bary.y;
+
+    float sign_bezierInside = d.x > d.y ? sign(d.x * d.x - d.y) : 1.0;
+
+    bvec3 cond = bvec3( p.y >= A.y,
+                        p.y <  C.y,
+                        a.x * c.y > a.y * c.x );
+    float signLineLeft = all(cond) || all(not(cond)) ? -1.0 : 1.0;
+
+    return sign_bezierInside * signLineLeft;
+}
+
+vec3 solve_cubic(float a, float b, float c)
+{
+    float p = b - a * a / 3.0, p3 = p * p * p;
+    float q = a * (2.0 * a * a - 9.0 * b) / 27.0 + c;
+    float d = q * q + 4.0 * p3 / 27.0;
+    float offset = -a / 3.0;
+    if(d >= 0.0) {
+        float z = sqrt(d);
+        vec2 x = (vec2(z, -z) - q) / 2.0;
+        vec2 uv = sign(x) * pow(abs(x), vec2(1.0 / 3.0));
+        return vec3(offset + uv.x + uv.y);
+    }
+    float v = acos(-sqrt(-27.0 / p3) * q / 2.0) / 3.0;
+    float m = cos(v), n = sin(v) * 1.732050808;
+    return vec3(m + m, -n - m, n - m) * sqrt(-p / 3.0) + offset;
+}
+
+float distance_bezier(vec2 A, vec2 B, vec2 C, vec2 p)
+{
+    B = mix(B + vec2(1e-4), B, abs(sign(B * 2.0 - A - C)));
+    vec2 a = B - A, b = A - B * 2.0 + C, c = a * 2.0, d = A - p;
+    vec3 k = vec3(3. * dot(a, b),2. * dot(a, a) + dot(d, b),dot(d, a)) / dot(b, b);
+    vec3 t = clamp(solve_cubic(k.x, k.y, k.z), 0.0, 1.0);
+    vec2 pos = A + (c + b * t.x) * t.x;
+    float dis = length(pos - p);
+    pos = A + (c + b * t.y) * t.y;
+    dis = min(dis, length(pos - p));
+    pos = A + (c + b * t.z) * t.z;
+    dis = min(dis, length(pos - p));
+    return dis;
+}
+
+void get_subpath_attr(
+    int start_idx,
+    out int end_idx,
+    out int idx,
+    out float d,
+    out float sgn
+) {
+    const int lim = (points.length() - 1) / 2 * 2;
+    end_idx = lim;
+    bool is_closed = get_isclosed(start_idx);
+
+    d = INFINITY;
+    sgn = 1.0;
+    for (int i = start_idx; i < lim; i += 2) {
+        vec2 B = get_point(i + 1);
+        if (isnan(B.x)) {
+            end_idx = i;
+            break;
+        }
+        vec2 A = get_point(i), C = get_point(i + 2);
+        if (A == B && B == C)
+            continue;
+
+        vec2 v1 = normalize(B - A);
+        vec2 v2 = normalize(C - B);
+        // REFACTOR: 使用更好的判断可近似为直线的方法
+        if (abs(cross2d(v1, v2)) < 1e-3 && dot(v1, v2) > 0.0) {
+            vec2 e = C - A;
+            vec2 w = v_coord - A;
+            vec2 b = w - e * clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
+            float dist = length(b);
+            if (dist < d) {
+                d = dist;
+                idx = i;
+            }
+
+            if (is_closed) {
+                bvec3 cond = bvec3( v_coord.y >= A.y,
+                                    v_coord.y  < C.y,
+                                    e.x * w.y > e.y * w.x );
+                if(all(cond) || all(not(cond))) sgn = -sgn;
+            }
+        } else {
+            float dist = distance_bezier(A, B, C, v_coord);
+            if (dist < d) {
+                d = dist;
+                idx = i;
+            }
+
+            if (is_closed) {
+                sgn *= sign_bezier(A, B, C, v_coord);
+            }
+        }
+    }
+}
+
+// #define CONTROL_POINTS
+// #define POLYGON_LINES
+// #define SDF_PLANE
+
+void main()
+{
+    float d;
+
+    #ifdef CONTROL_POINTS
+
+    d = distance(v_coord, get_point(0));
+    for (int i = 1; i < points.length(); i++) {
+        d = min(d, distance(v_coord, get_point(i)));
+    }
+    if (d < 0.06) {
+        f_color = vec4(1.0 - smoothstep(0.048, 0.052, d));
+        return;
+    }
+
+    #endif
+
+    int idx;
+    d = INFINITY;
+    float sgn = 1.0;
+
+    int start_idx = 0;
+    float sp_d;
+    float sp_sgn;
+
+    const int lim = (points.length() - 1) / 2 * 2;
+
+    while (true) {
+        get_subpath_attr(start_idx, start_idx, idx, sp_d, sp_sgn);
+        d = min(d, sp_d);
+        sgn *= sp_sgn;
+
+        if (start_idx >= lim)
+            break;
+        start_idx += 2;
+    }
+    int anchor_idx = idx / 2;
+    float sgn_d = sgn * d;
+
+    vec2 e = get_point(idx + 2) - get_point(idx);
+    vec2 w = v_coord - get_point(idx);
+    float ratio = clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
+
+    float radius = mix(get_radius(anchor_idx), get_radius(anchor_idx + 1), ratio);
+
+    vec4 fill_color = get_isclosed(idx) ? mix(fills[anchor_idx], fills[anchor_idx + 1], ratio) : vec4(0.0);
+    fill_color.a *= smoothstep(1, -1, (sgn_d) / JA_ANTI_ALIAS_RADIUS);
+
+    vec4 stroke_color = mix(colors[anchor_idx], colors[anchor_idx + 1], ratio);
+    stroke_color.a *= smoothstep(1, -1, (d - radius) / JA_ANTI_ALIAS_RADIUS);
+
+    f_color = blend_color(stroke_color, fill_color);
+
+    #if !defined(POLYGON_LINES) && !defined(SDF_PLANE)
+    if (f_color.a == 0.0)
+        discard;
+    #endif
+
+    #ifdef SDF_PLANE
+
+    vec4 df_color = vec4(1.0) - sgn * vec4(0.1, 0.4, 0.7, 0.0);
+    df_color *= 0.8 + 0.2 * cos(140. * d / 3.0);
+    df_color = mix(df_color, vec4(1.0), 1.0 - smoothstep(0.0, 0.02, abs(d)));
+    df_color.a = 0.5;
+    f_color = blend_color(df_color, f_color);
+
+    #endif
+
+    #ifdef POLYGON_LINES
+
+    const int num = points.length();
+    d = dot(v_coord - get_point(0), v_coord - get_point(0));
+    for(int i = 1, j = 0; i < num; j = i, i++)
+    {
+        if (get_point(j) == get_point(i)) {
+            i++;
+            continue;
+        }
+        // distance
+        vec2 e = get_point(j) - get_point(i);
+        vec2 w = v_coord - get_point(i);
+        vec2 b = w - e * clamp(dot(w, e) / dot(e, e), 0.0, 1.0);
+        d = min(d, dot(b, b));
+    }
+    float line_ratio = smoothstep(1.15, 0.85, sqrt(d) / 0.02);
+    f_color.g = max(line_ratio, f_color.g);
+    f_color.a = max(line_ratio, f_color.a);
+
+    #endif
 }
```

### Comparing `janim-1.0.4/janim/render/texture.py` & `janim-1.1.0/janim/render/texture.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-
-import moderngl as mgl
-from PIL import Image
-
-from janim.render.base import Renderer
-from janim.utils.file_ops import find_file
-
-filepath_to_img_map: dict[str, Image.Image] = {}
-
-
-def get_img_from_file(file_path: str) -> Image.Image:
-    file_path = find_file(file_path)
-    mtime = os.path.getmtime(file_path)
-    key = (file_path, mtime)
-
-    img = filepath_to_img_map.get(key, None)
-    if img is not None:
-        return img
-    img = Image.open(file_path).convert('RGBA')
-    filepath_to_img_map[key] = img
-    return img
-
-
-img_to_texture_map: dict[int, mgl.Texture] = {}
-
-
-def get_texture_from_img(img: Image.Image) -> mgl.Texture:
-    ctx = Renderer.data_ctx.get().ctx
-    key = (ctx, id(img))
-    texture = img_to_texture_map.get(key, None)
-    if texture is not None:
-        return texture
-    texture = ctx.texture(
-        size=img.size,
-        components=len(img.getbands()),
-        data=img.tobytes()
-    )
-    texture.repeat_x = False
-    texture.repeat_y = False
-    img_to_texture_map[key] = texture
-    return texture
+import os
+
+import moderngl as mgl
+from PIL import Image
+
+from janim.render.base import Renderer
+from janim.utils.file_ops import find_file
+
+filepath_to_img_map: dict[str, Image.Image] = {}
+
+
+def get_img_from_file(file_path: str) -> Image.Image:
+    file_path = find_file(file_path)
+    mtime = os.path.getmtime(file_path)
+    key = (file_path, mtime)
+
+    img = filepath_to_img_map.get(key, None)
+    if img is not None:
+        return img
+    img = Image.open(file_path).convert('RGBA')
+    filepath_to_img_map[key] = img
+    return img
+
+
+img_to_texture_map: dict[tuple[mgl.Context, int], mgl.Texture] = {}
+
+
+def get_texture_from_img(img: Image.Image) -> mgl.Texture:
+    ctx = Renderer.data_ctx.get().ctx
+    key = (ctx, id(img))
+    texture = img_to_texture_map.get(key, None)
+    if texture is not None:
+        return texture
+    texture = ctx.texture(
+        size=img.size,
+        components=len(img.getbands()),
+        data=img.tobytes()
+    )
+    texture.repeat_x = False
+    texture.repeat_y = False
+    img_to_texture_map[key] = texture
+    return texture
```

### Comparing `janim-1.0.4/janim/render/writer.py` & `janim-1.1.0/janim/render/writer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-import os
-import shutil
-import subprocess as sp
-import time
-from functools import partial
-
-import moderngl as mgl
-from tqdm import tqdm as ProgressDisplay
-
-from janim.anims.timeline import TimelineAnim
-from janim.exception import EXITCODE_FFMPEG_NOT_FOUND, ExitException
-from janim.logger import log
-
-
-class VideoWriter:
-    '''
-    将时间轴动画生成视频输出到文件中
-
-    可以直接调用 ``VideoWriter.writes(MyTimeline().build())`` 进行输出
-
-    主要流程在 :meth:`write_all` 中：
-
-    - 首先调用 ffmpeg，这里用它生成视频（先输出到 _temp 文件中）
-    - 然后遍历动画的每一帧，进行渲染，并将像素数据传递给 ffmpeg
-    - 最后结束 ffmpeg 的调用，完成 _temp 文件的输出
-    - 将 _temp 文件改名，删去 "_temp" 后缀，完成视频输出
-    '''
-    def __init__(self, anim: TimelineAnim):
-        self.anim = anim
-        self.ctx = mgl.create_standalone_context()
-        self.ctx.enable(mgl.BLEND)
-        self.ctx.blend_func = (
-            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
-            mgl.ONE, mgl.ONE
-        )
-        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
-
-        pw, ph = anim.cfg.pixel_width, anim.cfg.pixel_height
-        self.fbo = self.ctx.framebuffer(
-            color_attachments=self.ctx.texture(
-                (pw, ph),
-                components=4,
-                samples=0,
-            ),
-            depth_attachment=self.ctx.depth_renderbuffer(
-                (pw, ph),
-                samples=0
-            )
-        )
-
-    def write_all(self, file_path: str, *, quiet=False) -> None:
-        '''将时间轴动画输出到文件中
-
-        - 指定 ``quiet=True``，则不会输出前后的提示信息，但仍有进度条
-        '''
-        name = self.anim.timeline.__class__.__name__
-        if not quiet:
-            log.info(f'Writing "{name}"')
-            t = time.time()
-
-        self.fbo.use()
-        fps = self.anim.cfg.fps
-
-        self.open_video_pipe(file_path)
-
-        progress_display = ProgressDisplay(
-            range(round(self.anim.global_range.duration * fps) + 1),
-            leave=False,
-            dynamic_ncols=True
-        )
-
-        rgb = self.anim.cfg.background_color.rgb
-
-        for frame in progress_display:
-            self.fbo.clear(*rgb)
-            self.anim.anim_on(frame / fps)
-            self.anim.render_all(self.ctx)
-            bytes = self.fbo.read(components=4)
-            self.writing_process.stdin.write(bytes)
-
-        self.close_video_pipe()
-
-        if not quiet:
-            log.info(f'Finished writing "{name}" in {time.time() - t:.2f} s')
-            log.info(f'File saved to "{file_path}"')
-
-    def open_video_pipe(self, file_path: str) -> None:
-        stem, ext = os.path.splitext(file_path)
-        self.final_file_path = file_path
-        self.temp_file_path = stem + '_temp' + ext
-
-        command = [
-            self.anim.cfg.ffmpeg_bin,
-            '-y',   # overwrite output file if it exists
-            '-f', 'rawvideo',
-            '-s', f'{self.anim.cfg.pixel_width}x{self.anim.cfg.pixel_height}',  # size of one frame
-            '-pix_fmt', 'rgba',
-            '-r', str(self.anim.cfg.fps),  # frames per second
-            '-i', '-',  # The input comes from a pipe
-            '-vf', 'vflip',
-            '-an',  # Tells FFMPEG not to expect any audio
-            '-loglevel', 'error',
-        ]
-
-        if ext == ".mov":
-            # This is if the background of the exported
-            # video should be transparent.
-            command += [
-                '-vcodec', 'qtrle',
-            ]
-        else:
-            command += [
-                '-vcodec', 'libx264',
-                '-pix_fmt', 'yuv420p',
-            ]
-
-        command += [self.temp_file_path]
-        try:
-            self.writing_process = sp.Popen(command, stdin=sp.PIPE)
-        except FileNotFoundError:
-            log.error('无法输出视频，需要安装 ffmpeg 并将其添加到环境变量中')
-            raise ExitException(EXITCODE_FFMPEG_NOT_FOUND)
-
-    def close_video_pipe(self) -> None:
-        self.writing_process.stdin.close()
-        self.writing_process.wait()
-        self.writing_process.terminate()
-        shutil.move(self.temp_file_path, self.final_file_path)
-
-    @staticmethod
-    def writes(anim: TimelineAnim, file_path: str, *, quiet=False) -> None:
-        VideoWriter(anim).write_all(file_path, quiet=quiet)
-
-
-class AudioWriter:
-    def __init__(self, anim: TimelineAnim):
-        self.anim = anim
-
-    def write_all(self, file_path: str, *, quiet=False) -> None:
-        name = self.anim.timeline.__class__.__name__
-        if not quiet:
-            log.info(f'Writing audio of "{name}"')
-            t = time.time()
-
-        fps = self.anim.cfg.fps
-        framerate = self.anim.cfg.audio_framerate
-
-        self.open_audio_pipe(file_path)
-
-        progress_display = ProgressDisplay(
-            range(round(self.anim.global_range.duration * fps) + 1),
-            leave=False,
-            dynamic_ncols=True
-        )
-
-        get_audio_samples = partial(self.anim.timeline.get_audio_samples_of_frame,
-                                    fps,
-                                    framerate)
-
-        for frame in progress_display:
-            samples = get_audio_samples(frame)
-            self.writing_process.stdin.write(samples.tobytes())
-
-        self.close_audio_pipe()
-
-        if not quiet:
-            log.info(f'Finished writing audio of "{name}" in {time.time() - t:.2f} s')
-            log.info(f'File saved to "{file_path}"')
-
-    def open_audio_pipe(self, file_path: str) -> None:
-        stem, ext = os.path.splitext(file_path)
-        self.final_file_path = file_path
-        self.temp_file_path = stem + '_temp' + ext
-
-        command = [
-            self.anim.cfg.ffmpeg_bin,
-            '-y',   # overwrite output file if it exists
-            '-f', 's16le',
-            '-ar', str(self.anim.cfg.audio_framerate),     # framerate & samplerate
-            '-ac', '1',
-            '-i', '-',
-            '-loglevel', 'error',
-            self.temp_file_path
-        ]
-
-        try:
-            self.writing_process = sp.Popen(command, stdin=sp.PIPE)
-        except FileNotFoundError:
-            log.error('无法输出音频，需要安装 ffmpeg 并将其添加到环境变量中')
-            raise ExitException(EXITCODE_FFMPEG_NOT_FOUND)
-
-    def close_audio_pipe(self) -> None:
-        self.writing_process.stdin.close()
-        self.writing_process.wait()
-        self.writing_process.terminate()
-        shutil.move(self.temp_file_path, self.final_file_path)
-
-    @staticmethod
-    def writes(anim: TimelineAnim, file_path: str, *, quiet=False) -> None:
-        AudioWriter(anim).write_all(file_path, quiet=quiet)
+import os
+import shutil
+import subprocess as sp
+import time
+from functools import partial
+
+import moderngl as mgl
+from tqdm import tqdm as ProgressDisplay
+
+from janim.anims.timeline import TimelineAnim
+from janim.exception import EXITCODE_FFMPEG_NOT_FOUND, ExitException
+from janim.logger import log
+
+
+class VideoWriter:
+    '''
+    将时间轴动画生成视频输出到文件中
+
+    可以直接调用 ``VideoWriter.writes(MyTimeline().build())`` 进行输出
+
+    主要流程在 :meth:`write_all` 中：
+
+    - 首先调用 ffmpeg，这里用它生成视频（先输出到 _temp 文件中）
+    - 然后遍历动画的每一帧，进行渲染，并将像素数据传递给 ffmpeg
+    - 最后结束 ffmpeg 的调用，完成 _temp 文件的输出
+    - 将 _temp 文件改名，删去 "_temp" 后缀，完成视频输出
+    '''
+    def __init__(self, anim: TimelineAnim):
+        self.anim = anim
+        self.ctx = mgl.create_standalone_context()
+        self.ctx.enable(mgl.BLEND)
+        self.ctx.blend_func = (
+            mgl.SRC_ALPHA, mgl.ONE_MINUS_SRC_ALPHA,
+            mgl.ONE, mgl.ONE
+        )
+        self.ctx.blend_equation = mgl.FUNC_ADD, mgl.MAX
+
+        pw, ph = anim.cfg.pixel_width, anim.cfg.pixel_height
+        self.fbo = self.ctx.framebuffer(
+            color_attachments=self.ctx.texture(
+                (pw, ph),
+                components=4,
+                samples=0,
+            ),
+            depth_attachment=self.ctx.depth_renderbuffer(
+                (pw, ph),
+                samples=0
+            )
+        )
+
+    def write_all(self, file_path: str, *, quiet=False) -> None:
+        '''将时间轴动画输出到文件中
+
+        - 指定 ``quiet=True``，则不会输出前后的提示信息，但仍有进度条
+        '''
+        name = self.anim.timeline.__class__.__name__
+        if not quiet:
+            log.info(f'Writing "{name}"')
+            t = time.time()
+
+        self.fbo.use()
+        fps = self.anim.cfg.fps
+
+        self.open_video_pipe(file_path)
+
+        progress_display = ProgressDisplay(
+            range(round(self.anim.global_range.duration * fps) + 1),
+            leave=False,
+            dynamic_ncols=True
+        )
+
+        rgb = self.anim.cfg.background_color.rgb
+
+        for frame in progress_display:
+            self.fbo.clear(*rgb)
+            self.anim.anim_on(frame / fps)
+            self.anim.render_all(self.ctx)
+            bytes = self.fbo.read(components=4)
+            self.writing_process.stdin.write(bytes)
+
+        self.close_video_pipe()
+
+        if not quiet:
+            log.info(f'Finished writing "{name}" in {time.time() - t:.2f} s')
+            log.info(f'File saved to "{file_path}"')
+
+    def open_video_pipe(self, file_path: str) -> None:
+        stem, ext = os.path.splitext(file_path)
+        self.final_file_path = file_path
+        self.temp_file_path = stem + '_temp' + ext
+
+        command = [
+            self.anim.cfg.ffmpeg_bin,
+            '-y',   # overwrite output file if it exists
+            '-f', 'rawvideo',
+            '-s', f'{self.anim.cfg.pixel_width}x{self.anim.cfg.pixel_height}',  # size of one frame
+            '-pix_fmt', 'rgba',
+            '-r', str(self.anim.cfg.fps),  # frames per second
+            '-i', '-',  # The input comes from a pipe
+            '-vf', 'vflip',
+            '-an',  # Tells FFMPEG not to expect any audio
+            '-loglevel', 'error',
+        ]
+
+        if ext == ".mov":
+            # This is if the background of the exported
+            # video should be transparent.
+            command += [
+                '-vcodec', 'qtrle',
+            ]
+        else:
+            command += [
+                '-vcodec', 'libx264',
+                '-pix_fmt', 'yuv420p',
+            ]
+
+        command += [self.temp_file_path]
+        try:
+            self.writing_process = sp.Popen(command, stdin=sp.PIPE)
+        except FileNotFoundError:
+            log.error('无法输出视频，需要安装 ffmpeg 并将其添加到环境变量中')
+            raise ExitException(EXITCODE_FFMPEG_NOT_FOUND)
+
+    def close_video_pipe(self) -> None:
+        self.writing_process.stdin.close()
+        self.writing_process.wait()
+        self.writing_process.terminate()
+        shutil.move(self.temp_file_path, self.final_file_path)
+
+    @staticmethod
+    def writes(anim: TimelineAnim, file_path: str, *, quiet=False) -> None:
+        VideoWriter(anim).write_all(file_path, quiet=quiet)
+
+
+class AudioWriter:
+    def __init__(self, anim: TimelineAnim):
+        self.anim = anim
+
+    def write_all(self, file_path: str, *, quiet=False) -> None:
+        name = self.anim.timeline.__class__.__name__
+        if not quiet:
+            log.info(f'Writing audio of "{name}"')
+            t = time.time()
+
+        fps = self.anim.cfg.fps
+        framerate = self.anim.cfg.audio_framerate
+
+        self.open_audio_pipe(file_path)
+
+        progress_display = ProgressDisplay(
+            range(round(self.anim.global_range.duration * fps) + 1),
+            leave=False,
+            dynamic_ncols=True
+        )
+
+        get_audio_samples = partial(self.anim.timeline.get_audio_samples_of_frame,
+                                    fps,
+                                    framerate)
+
+        for frame in progress_display:
+            samples = get_audio_samples(frame)
+            self.writing_process.stdin.write(samples.tobytes())
+
+        self.close_audio_pipe()
+
+        if not quiet:
+            log.info(f'Finished writing audio of "{name}" in {time.time() - t:.2f} s')
+            log.info(f'File saved to "{file_path}"')
+
+    def open_audio_pipe(self, file_path: str) -> None:
+        stem, ext = os.path.splitext(file_path)
+        self.final_file_path = file_path
+        self.temp_file_path = stem + '_temp' + ext
+
+        command = [
+            self.anim.cfg.ffmpeg_bin,
+            '-y',   # overwrite output file if it exists
+            '-f', 's16le',
+            '-ar', str(self.anim.cfg.audio_framerate),     # framerate & samplerate
+            '-ac', '1',
+            '-i', '-',
+            '-loglevel', 'error',
+            self.temp_file_path
+        ]
+
+        try:
+            self.writing_process = sp.Popen(command, stdin=sp.PIPE)
+        except FileNotFoundError:
+            log.error('无法输出音频，需要安装 ffmpeg 并将其添加到环境变量中')
+            raise ExitException(EXITCODE_FFMPEG_NOT_FOUND)
+
+    def close_audio_pipe(self) -> None:
+        self.writing_process.stdin.close()
+        self.writing_process.wait()
+        self.writing_process.terminate()
+        shutil.move(self.temp_file_path, self.final_file_path)
+
+    @staticmethod
+    def writes(anim: TimelineAnim, file_path: str, *, quiet=False) -> None:
+        AudioWriter(anim).write_all(file_path, quiet=quiet)
```

### Comparing `janim-1.0.4/janim/typing.py` & `janim-1.1.0/janim/typing.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import TYPE_CHECKING, Iterable, Protocol, runtime_checkable
-
-from janim.utils.data import AlignedData
-
-if TYPE_CHECKING:
-    import numpy as np
-
-type Vect = Iterable[float] | np.ndarray
-type VectArray = Iterable[Vect] | np.ndarray
-
-type JAnimColor = str | Iterable[float] | np.ndarray
-type ColorArray = Iterable[JAnimColor] | np.ndarray
-
-type Alpha = float
-type AlphaArray = Iterable[float] | np.ndarray
-
-type Rgba = Iterable[float] | np.ndarray
-type RgbaArray = Iterable[Rgba] | np.ndarray
-
-type RangeSpecifier = tuple[float, float] | tuple[float, float, float]
-
-
-@runtime_checkable
-class SupportsInterpolate[T](Protocol):
-    @classmethod
-    def align_for_interpolate(cls, obj1: object, obj2: object) -> AlignedData[T]: ...
-
-    def interpolate(self, obj1: object, obj2: object, alpha: float, *, path_func): ...
-
-
-@runtime_checkable
-class SupportsApartAlpha(Protocol):
-    def apart_alpha(self, n: int) -> None: ...
+from typing import TYPE_CHECKING, Iterable, Protocol, runtime_checkable
+
+from janim.utils.data import AlignedData
+
+if TYPE_CHECKING:
+    import numpy as np
+
+type Vect = Iterable[float] | np.ndarray
+type VectArray = Iterable[Vect] | np.ndarray
+
+type JAnimColor = str | Iterable[float] | np.ndarray
+type ColorArray = Iterable[JAnimColor] | np.ndarray
+
+type Alpha = float
+type AlphaArray = Iterable[float] | np.ndarray
+
+type Rgba = Iterable[float] | np.ndarray
+type RgbaArray = Iterable[Rgba] | np.ndarray
+
+type RangeSpecifier = tuple[float, float] | tuple[float, float, float]
+
+
+@runtime_checkable
+class SupportsInterpolate[T](Protocol):
+    @classmethod
+    def align_for_interpolate(cls, obj1: object, obj2: object) -> AlignedData[T]: ...
+
+    def interpolate(self, obj1: object, obj2: object, alpha: float, *, path_func): ...
+
+
+@runtime_checkable
+class SupportsApartAlpha(Protocol):
+    def apart_alpha(self, n: int) -> None: ...
```

### Comparing `janim-1.0.4/janim/utils/dict_ops.py` & `janim-1.1.0/janim/utils/dict_ops.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import itertools as it
-
-
-def merge_dicts_recursively(*dicts: dict) -> dict:
-    '''
-    递归合并字典
-
-    - 创建一个字典，其键集是所有输入字典的并集
-    - 在列表中位置越靠后的字典具有更高的优先级
-    - 当值为字典时，将递归应用
-    '''
-    result = {}
-    all_items = it.chain(*[d.items() for d in dicts])
-    for key, value in all_items:
-        if key in result and isinstance(result[key], dict) and isinstance(value, dict):
-            result[key] = merge_dicts_recursively(result[key], value)
-        else:
-            result[key] = value
-    return result
+import itertools as it
+
+
+def merge_dicts_recursively(*dicts: dict) -> dict:
+    '''
+    递归合并字典
+
+    - 创建一个字典，其键集是所有输入字典的并集
+    - 在列表中位置越靠后的字典具有更高的优先级
+    - 当值为字典时，将递归应用
+    '''
+    result = {}
+    all_items = it.chain(*[d.items() for d in dicts])
+    for key, value in all_items:
+        if key in result and isinstance(result[key], dict) and isinstance(value, dict):
+            result[key] = merge_dicts_recursively(result[key], value)
+        else:
+            result[key] = value
+    return result
```

### Comparing `janim-1.0.4/janim/utils/font_manager.py` & `janim-1.1.0/janim/utils/font_manager.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-# borrowed from matplotlib.font_manager
-
-import sys
-import os
-import logging
-import subprocess
-from functools import lru_cache
-from pathlib import Path
-
-_log = logging.getLogger(__name__)
-
-
-# OS Font paths
-try:
-    _HOME = Path.home()
-except Exception:  # Exceptions thrown by home() are not specified...
-    _HOME = Path(os.devnull)  # Just an arbitrary path with no children.
-MSFolders = \
-    r'Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders'
-MSFontDirectories = [
-    r'SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts',
-    r'SOFTWARE\Microsoft\Windows\CurrentVersion\Fonts']
-MSUserFontDirectories = [
-    str(_HOME / 'AppData/Local/Microsoft/Windows/Fonts'),
-    str(_HOME / 'AppData/Roaming/Microsoft/Windows/Fonts'),
-]
-X11FontDirectories = [
-    # an old standard installation point
-    "/usr/X11R6/lib/X11/fonts/TTF/",
-    "/usr/X11/lib/X11/fonts",
-    # here is the new standard location for fonts
-    "/usr/share/fonts/",
-    # documented as a good place to install new fonts
-    "/usr/local/share/fonts/",
-    # common application, not really useful
-    "/usr/lib/openoffice/share/fonts/truetype/",
-    # user fonts
-    str((Path(os.environ.get('XDG_DATA_HOME') or _HOME / ".local/share"))
-        / "fonts"),
-    str(_HOME / ".fonts"),
-]
-OSXFontDirectories = [
-    "/Library/Fonts/",
-    "/Network/Library/Fonts/",
-    "/System/Library/Fonts/",
-    # fonts installed via MacPorts
-    "/opt/local/share/fonts",
-    # user fonts
-    str(_HOME / "Library/Fonts"),
-]
-
-
-@lru_cache(64)
-def _cached_realpath(path):
-    return os.path.realpath(path)
-
-
-def get_fontext_synonyms(fontext):
-    """
-    Return a list of file extensions extensions that are synonyms for
-    the given file extension *fileext*.
-    """
-    return {
-        'afm': ['afm'],
-        'otf': ['otf', 'ttc', 'ttf'],
-        'ttc': ['otf', 'ttc', 'ttf'],
-        'ttf': ['otf', 'ttc', 'ttf'],
-    }[fontext]
-
-
-def list_fonts(directory, extensions):
-    """
-    Return a list of all fonts matching any of the extensions, found
-    recursively under the directory.
-    """
-    extensions = ["." + ext for ext in extensions]
-    return [os.path.join(dirpath, filename)
-            # os.walk ignores access errors, unlike Path.glob.
-            for dirpath, _, filenames in os.walk(directory)
-            for filename in filenames
-            if Path(filename).suffix.lower() in extensions]
-
-
-def win32FontDirectory():
-    r"""
-    Return the user-specified font directory for Win32.  This is
-    looked up from the registry key ::
-
-      \\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders\Fonts
-
-    If the key is not found, ``%WINDIR%\Fonts`` will be returned.
-    """
-    import winreg
-    try:
-        with winreg.OpenKey(winreg.HKEY_CURRENT_USER, MSFolders) as user:
-            return winreg.QueryValueEx(user, 'Fonts')[0]
-    except OSError:
-        return os.path.join(os.environ['WINDIR'], 'Fonts')
-
-
-def _get_win32_installed_fonts():
-    """List the font paths known to the Windows registry."""
-    import winreg
-    items = set()
-    # Search and resolve fonts listed in the registry.
-    for domain, base_dirs in [
-            (winreg.HKEY_LOCAL_MACHINE, [win32FontDirectory()]),  # System.
-            (winreg.HKEY_CURRENT_USER, MSUserFontDirectories),  # User.
-    ]:
-        for base_dir in base_dirs:
-            for reg_path in MSFontDirectories:
-                try:
-                    with winreg.OpenKey(domain, reg_path) as local:
-                        for j in range(winreg.QueryInfoKey(local)[1]):
-                            # value may contain the filename of the font or its
-                            # absolute path.
-                            key, value, tp = winreg.EnumValue(local, j)
-                            if not isinstance(value, str):
-                                continue
-                            try:
-                                # If value contains already an absolute path,
-                                # then it is not changed further.
-                                path = Path(base_dir, value).resolve()
-                            except RuntimeError:
-                                # Don't fail with invalid entries.
-                                continue
-                            items.add(path)
-                except (OSError, MemoryError):
-                    continue
-    return items
-
-
-@lru_cache()
-def _get_fontconfig_fonts():
-    """Cache and list the font paths known to `fc-list`."""
-    try:
-        if b'--format' not in subprocess.check_output(['fc-list', '--help']):
-            _log.warning(  # fontconfig 2.7 implemented --format.
-                'needs fontconfig>=2.7 to query system fonts.')
-            return []
-        out = subprocess.check_output(['fc-list', '--format=%{file}\\n'])
-    except (OSError, subprocess.CalledProcessError):
-        return []
-    return [Path(os.fsdecode(fname)) for fname in out.split(b'\n')]
-
-
-def findSystemFonts(fontpaths=None, fontext='ttf'):
-    """
-    Search for fonts in the specified font paths.  If no paths are
-    given, will use a standard set of system paths, as well as the
-    list of fonts tracked by fontconfig if fontconfig is installed and
-    available.  A list of TrueType fonts are returned by default with
-    AFM fonts as an option.
-    """
-    fontfiles = set()
-    fontexts = get_fontext_synonyms(fontext)
-
-    if fontpaths is None:
-        if sys.platform == 'win32':
-            installed_fonts = _get_win32_installed_fonts()
-            fontpaths = MSUserFontDirectories + [win32FontDirectory()]
-        else:
-            installed_fonts = _get_fontconfig_fonts()
-            if sys.platform == 'darwin':
-                fontpaths = [*X11FontDirectories, *OSXFontDirectories]
-            else:
-                fontpaths = X11FontDirectories
-        fontfiles.update(str(path) for path in installed_fonts
-                         if path.suffix.lower()[1:] in fontexts)
-
-    elif isinstance(fontpaths, str):
-        fontpaths = [fontpaths]
-
-    for path in fontpaths:
-        fontfiles.update(map(os.path.abspath, list_fonts(path, fontexts)))
-
-    return [fname for fname in fontfiles if os.path.exists(fname)]
+# borrowed from matplotlib.font_manager
+
+import sys
+import os
+import logging
+import subprocess
+from functools import lru_cache
+from pathlib import Path
+
+_log = logging.getLogger(__name__)
+
+
+# OS Font paths
+try:
+    _HOME = Path.home()
+except Exception:  # Exceptions thrown by home() are not specified...
+    _HOME = Path(os.devnull)  # Just an arbitrary path with no children.
+MSFolders = \
+    r'Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders'
+MSFontDirectories = [
+    r'SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts',
+    r'SOFTWARE\Microsoft\Windows\CurrentVersion\Fonts']
+MSUserFontDirectories = [
+    str(_HOME / 'AppData/Local/Microsoft/Windows/Fonts'),
+    str(_HOME / 'AppData/Roaming/Microsoft/Windows/Fonts'),
+]
+X11FontDirectories = [
+    # an old standard installation point
+    "/usr/X11R6/lib/X11/fonts/TTF/",
+    "/usr/X11/lib/X11/fonts",
+    # here is the new standard location for fonts
+    "/usr/share/fonts/",
+    # documented as a good place to install new fonts
+    "/usr/local/share/fonts/",
+    # common application, not really useful
+    "/usr/lib/openoffice/share/fonts/truetype/",
+    # user fonts
+    str((Path(os.environ.get('XDG_DATA_HOME') or _HOME / ".local/share"))
+        / "fonts"),
+    str(_HOME / ".fonts"),
+]
+OSXFontDirectories = [
+    "/Library/Fonts/",
+    "/Network/Library/Fonts/",
+    "/System/Library/Fonts/",
+    # fonts installed via MacPorts
+    "/opt/local/share/fonts",
+    # user fonts
+    str(_HOME / "Library/Fonts"),
+]
+
+
+@lru_cache(64)
+def _cached_realpath(path):
+    return os.path.realpath(path)
+
+
+def get_fontext_synonyms(fontext):
+    """
+    Return a list of file extensions extensions that are synonyms for
+    the given file extension *fileext*.
+    """
+    return {
+        'afm': ['afm'],
+        'otf': ['otf', 'ttc', 'ttf'],
+        'ttc': ['otf', 'ttc', 'ttf'],
+        'ttf': ['otf', 'ttc', 'ttf'],
+    }[fontext]
+
+
+def list_fonts(directory, extensions):
+    """
+    Return a list of all fonts matching any of the extensions, found
+    recursively under the directory.
+    """
+    extensions = ["." + ext for ext in extensions]
+    return [os.path.join(dirpath, filename)
+            # os.walk ignores access errors, unlike Path.glob.
+            for dirpath, _, filenames in os.walk(directory)
+            for filename in filenames
+            if Path(filename).suffix.lower() in extensions]
+
+
+def win32FontDirectory():
+    r"""
+    Return the user-specified font directory for Win32.  This is
+    looked up from the registry key ::
+
+      \\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders\Fonts
+
+    If the key is not found, ``%WINDIR%\Fonts`` will be returned.
+    """
+    import winreg
+    try:
+        with winreg.OpenKey(winreg.HKEY_CURRENT_USER, MSFolders) as user:
+            return winreg.QueryValueEx(user, 'Fonts')[0]
+    except OSError:
+        return os.path.join(os.environ['WINDIR'], 'Fonts')
+
+
+def _get_win32_installed_fonts():
+    """List the font paths known to the Windows registry."""
+    import winreg
+    items = set()
+    # Search and resolve fonts listed in the registry.
+    for domain, base_dirs in [
+            (winreg.HKEY_LOCAL_MACHINE, [win32FontDirectory()]),  # System.
+            (winreg.HKEY_CURRENT_USER, MSUserFontDirectories),  # User.
+    ]:
+        for base_dir in base_dirs:
+            for reg_path in MSFontDirectories:
+                try:
+                    with winreg.OpenKey(domain, reg_path) as local:
+                        for j in range(winreg.QueryInfoKey(local)[1]):
+                            # value may contain the filename of the font or its
+                            # absolute path.
+                            key, value, tp = winreg.EnumValue(local, j)
+                            if not isinstance(value, str):
+                                continue
+                            try:
+                                # If value contains already an absolute path,
+                                # then it is not changed further.
+                                path = Path(base_dir, value).resolve()
+                            except RuntimeError:
+                                # Don't fail with invalid entries.
+                                continue
+                            items.add(path)
+                except (OSError, MemoryError):
+                    continue
+    return items
+
+
+@lru_cache()
+def _get_fontconfig_fonts():
+    """Cache and list the font paths known to `fc-list`."""
+    try:
+        if b'--format' not in subprocess.check_output(['fc-list', '--help']):
+            _log.warning(  # fontconfig 2.7 implemented --format.
+                'needs fontconfig>=2.7 to query system fonts.')
+            return []
+        out = subprocess.check_output(['fc-list', '--format=%{file}\\n'])
+    except (OSError, subprocess.CalledProcessError):
+        return []
+    return [Path(os.fsdecode(fname)) for fname in out.split(b'\n')]
+
+
+def findSystemFonts(fontpaths=None, fontext='ttf'):
+    """
+    Search for fonts in the specified font paths.  If no paths are
+    given, will use a standard set of system paths, as well as the
+    list of fonts tracked by fontconfig if fontconfig is installed and
+    available.  A list of TrueType fonts are returned by default with
+    AFM fonts as an option.
+    """
+    fontfiles = set()
+    fontexts = get_fontext_synonyms(fontext)
+
+    if fontpaths is None:
+        if sys.platform == 'win32':
+            installed_fonts = _get_win32_installed_fonts()
+            fontpaths = MSUserFontDirectories + [win32FontDirectory()]
+        else:
+            installed_fonts = _get_fontconfig_fonts()
+            if sys.platform == 'darwin':
+                fontpaths = [*X11FontDirectories, *OSXFontDirectories]
+            else:
+                fontpaths = X11FontDirectories
+        fontfiles.update(str(path) for path in installed_fonts
+                         if path.suffix.lower()[1:] in fontexts)
+
+    elif isinstance(fontpaths, str):
+        fontpaths = [fontpaths]
+
+    for path in fontpaths:
+        fontfiles.update(map(os.path.abspath, list_fonts(path, fontexts)))
+
+    return [fname for fname in fontfiles if os.path.exists(fname)]
```

### Comparing `janim-1.0.4/janim/utils/iterables.py` & `janim-1.1.0/janim/utils/iterables.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from __future__ import annotations
-
-import types
-from typing import Callable, Iterable, Sequence, TypeVar, overload
-
-import numpy as np
-
-T = TypeVar("T")
-S = TypeVar("S")
-
-type ResizeFunc = Callable[[np.ndarray, int], np.ndarray]
-
-
-def remove_list_redundancies(lst: Iterable[T]) -> list[T]:
-    """
-    Used instead of list(set(l)) to maintain order
-    Keeps the last occurrence of each element
-    """
-    reversed_result = []
-    used = set()
-    for x in reversed(lst):
-        if x not in used:
-            reversed_result.append(x)
-            used.add(x)
-    reversed_result.reverse()
-    return reversed_result
-
-
-def list_update(l1: Iterable[T], l2: Iterable[T]) -> list[T]:
-    """
-    Used instead of list(set(l1).update(l2)) to maintain order,
-    making sure duplicates are removed from l1, not l2.
-    """
-    return [e for e in l1 if e not in l2] + list(l2)
-
-
-def list_difference_update(l1: Iterable[T], l2: Iterable[T]) -> list[T]:
-    return [e for e in l1 if e not in l2]
-
-
-def adjacent_n_tuples(objects: Iterable[T], n: int) -> zip[tuple[T, T]]:
-    return zip(*[
-        [*objects[k:], *objects[:k]]
-        for k in range(n)
-    ])
-
-
-def adjacent_pairs(objects: Iterable[T]) -> zip[tuple[T, T]]:
-    return adjacent_n_tuples(objects, 2)
-
-
-def batch_by_property(
-    items: Iterable[T],
-    property_func: Callable[[T], S]
-) -> list[tuple[T, S]]:
-    """
-    Takes in a list, and returns a list of tuples, (batch, prop)
-    such that all items in a batch have the same output when
-    put into property_func, and such that chaining all these
-    batches together would give the original list (i.e. order is
-    preserved)
-    """
-    batch_prop_pairs = []
-    curr_batch = []
-    curr_prop = None
-    for item in items:
-        prop = property_func(item)
-        if prop != curr_prop:
-            # Add current batch
-            if len(curr_batch) > 0:
-                batch_prop_pairs.append((curr_batch, curr_prop))
-            # Redefine curr
-            curr_prop = prop
-            curr_batch = [item]
-        else:
-            curr_batch.append(item)
-    if len(curr_batch) > 0:
-        batch_prop_pairs.append((curr_batch, curr_prop))
-    return batch_prop_pairs
-
-
-def listify(obj) -> list:
-    if isinstance(obj, str):
-        return [obj]
-    try:
-        return list(obj)
-    except TypeError:
-        return [obj]
-
-
-def resize_array(nparray: np.ndarray, length: int) -> np.ndarray:
-    if len(nparray) == length:
-        return nparray
-    return np.resize(nparray, (length, *nparray.shape[1:]))
-
-
-@overload
-def resize_preserving_order(array: np.ndarray, length: int) -> np.ndarray: ...
-@overload
-def resize_preserving_order[T](array: list[T], length: int, fall_back: Callable = types.NoneType) -> list[T]: ...
-
-
-def resize_preserving_order(
-    array: np.ndarray | list[T],
-    length: int,
-    fall_back: Callable = types.NoneType
-):
-    if isinstance(array, np.ndarray):
-        if len(array) == 0:
-            return np.zeros((0, *array.shape[1:]), dtype=array.dtype)
-        if len(array) == length:
-            return array
-        indices = np.arange(length) * len(array) // length
-        return array[indices]
-
-    else:  # not isinstance(array, np.ndarray)
-        if len(array) == 0:
-            return [fall_back() for _ in range(length)]
-        if len(array) == length:
-            return array
-        indices = np.arange(length) * len(array) // length
-        return [array[idx] for idx in indices]
-
-
-def resize_preserving_order_indice_groups(len1: int, len2: int) -> list[list[int]]:
-    indices = np.arange(len2) * len1 // len2
-    result = []
-    prev = 0
-    current = []
-    for i, indice in enumerate(indices):
-        if prev != indice:
-            prev = indice
-            result.append(current)
-            current = []
-
-        current.append(i)
-
-    result.append(current)
-
-    return result
-
-
-def resize_and_repeatedly_extend(
-    array: np.ndarray,
-    length: int,
-    fall_back: Callable[[int], np.ndarray] = lambda length: np.zeros((length, 3))
-) -> np.ndarray:
-    '''
-    注意：这个函数在 length <= len(array) 时，不会产生 array 的拷贝
-    '''
-    if length == len(array):
-        return array
-
-    if length < len(array):
-        return array[:length]
-
-    elif length > len(array):
-        if len(array) == 0:
-            return fall_back(length)
-
-        # len(array) != 0
-        return np.vstack([
-            array,
-            np.repeat([array[-1]], length - len(array), axis=0)
-        ])
-
-
-def resize_with_interpolation(nparray: np.ndarray, length: int) -> np.ndarray:
-    if not isinstance(nparray, np.ndarray):
-        nparray = np.array(nparray)
-    if len(nparray) == length:
-        return nparray
-    if length == 0:
-        return np.zeros((0, *nparray.shape[1:]))
-    cont_indices = np.linspace(0, len(nparray) - 1, length)
-    lh_s = cont_indices.astype(int)
-    rh_s = np.ceil(cont_indices).astype(int)
-    a_s = cont_indices % 1
-    a_s = np.expand_dims(a_s, axis=tuple(range(1, nparray.ndim)))
-    return (1 - a_s) * nparray[lh_s] + a_s * nparray[rh_s]
-
-
-def make_even(
-    iterable_1: Sequence[T],
-    iterable_2: Sequence[S]
-) -> tuple[list[T], list[S]]:
-    len1 = len(iterable_1)
-    len2 = len(iterable_2)
-    if len1 == len2:
-        return iterable_1, iterable_2
-    new_len = max(len1, len2)
-    return (
-        [iterable_1[(n * len1) // new_len] for n in range(new_len)],
-        [iterable_2[(n * len2) // new_len] for n in range(new_len)]
-    )
-
-
-def hash_obj(obj: object) -> int:
-    if isinstance(obj, dict):
-        new_obj = {k: hash_obj(v) for k, v in obj.items()}
-        return hash(tuple(frozenset(sorted(new_obj.items()))))
-
-    if isinstance(obj, (set, tuple, list)):
-        return hash(tuple(hash_obj(e) for e in obj))
-
-    return hash(obj)
+from __future__ import annotations
+
+import types
+from typing import Callable, Iterable, Sequence, TypeVar, overload
+
+import numpy as np
+
+T = TypeVar("T")
+S = TypeVar("S")
+
+type ResizeFunc = Callable[[np.ndarray, int], np.ndarray]
+
+
+def remove_list_redundancies(lst: Iterable[T]) -> list[T]:
+    """
+    Used instead of list(set(l)) to maintain order
+    Keeps the last occurrence of each element
+    """
+    reversed_result = []
+    used = set()
+    for x in reversed(lst):
+        if x not in used:
+            reversed_result.append(x)
+            used.add(x)
+    reversed_result.reverse()
+    return reversed_result
+
+
+def list_update(l1: Iterable[T], l2: Iterable[T]) -> list[T]:
+    """
+    Used instead of list(set(l1).update(l2)) to maintain order,
+    making sure duplicates are removed from l1, not l2.
+    """
+    return [e for e in l1 if e not in l2] + list(l2)
+
+
+def list_difference_update(l1: Iterable[T], l2: Iterable[T]) -> list[T]:
+    return [e for e in l1 if e not in l2]
+
+
+def adjacent_n_tuples(objects: Iterable[T], n: int) -> zip[tuple[T, T]]:
+    return zip(*[
+        [*objects[k:], *objects[:k]]
+        for k in range(n)
+    ])
+
+
+def adjacent_pairs(objects: Iterable[T]) -> zip[tuple[T, T]]:
+    return adjacent_n_tuples(objects, 2)
+
+
+def batch_by_property(
+    items: Iterable[T],
+    property_func: Callable[[T], S]
+) -> list[tuple[T, S]]:
+    """
+    Takes in a list, and returns a list of tuples, (batch, prop)
+    such that all items in a batch have the same output when
+    put into property_func, and such that chaining all these
+    batches together would give the original list (i.e. order is
+    preserved)
+    """
+    batch_prop_pairs = []
+    curr_batch = []
+    curr_prop = None
+    for item in items:
+        prop = property_func(item)
+        if prop != curr_prop:
+            # Add current batch
+            if len(curr_batch) > 0:
+                batch_prop_pairs.append((curr_batch, curr_prop))
+            # Redefine curr
+            curr_prop = prop
+            curr_batch = [item]
+        else:
+            curr_batch.append(item)
+    if len(curr_batch) > 0:
+        batch_prop_pairs.append((curr_batch, curr_prop))
+    return batch_prop_pairs
+
+
+def listify(obj) -> list:
+    if isinstance(obj, str):
+        return [obj]
+    try:
+        return list(obj)
+    except TypeError:
+        return [obj]
+
+
+def resize_array(nparray: np.ndarray, length: int) -> np.ndarray:
+    if len(nparray) == length:
+        return nparray
+    return np.resize(nparray, (length, *nparray.shape[1:]))
+
+
+@overload
+def resize_preserving_order(array: np.ndarray, length: int) -> np.ndarray: ...
+@overload
+def resize_preserving_order[T](array: list[T], length: int, fall_back: Callable = types.NoneType) -> list[T]: ...
+
+
+def resize_preserving_order(
+    array: np.ndarray | list[T],
+    length: int,
+    fall_back: Callable = types.NoneType
+):
+    if isinstance(array, np.ndarray):
+        if len(array) == 0:
+            return np.zeros((0, *array.shape[1:]), dtype=array.dtype)
+        if len(array) == length:
+            return array
+        indices = np.arange(length) * len(array) // length
+        return array[indices]
+
+    else:  # not isinstance(array, np.ndarray)
+        if len(array) == 0:
+            return [fall_back() for _ in range(length)]
+        if len(array) == length:
+            return array
+        indices = np.arange(length) * len(array) // length
+        return [array[idx] for idx in indices]
+
+
+def resize_preserving_order_indice_groups(len1: int, len2: int) -> list[list[int]]:
+    indices = np.arange(len2) * len1 // len2
+    result = []
+    prev = 0
+    current = []
+    for i, indice in enumerate(indices):
+        if prev != indice:
+            prev = indice
+            result.append(current)
+            current = []
+
+        current.append(i)
+
+    result.append(current)
+
+    return result
+
+
+def resize_and_repeatedly_extend(
+    array: np.ndarray,
+    length: int,
+    fall_back: Callable[[int], np.ndarray] = lambda length: np.zeros((length, 3))
+) -> np.ndarray:
+    '''
+    注意：这个函数在 length <= len(array) 时，不会产生 array 的拷贝
+    '''
+    if length == len(array):
+        return array
+
+    if length < len(array):
+        return array[:length]
+
+    elif length > len(array):
+        if len(array) == 0:
+            return fall_back(length)
+
+        # len(array) != 0
+        return np.vstack([
+            array,
+            np.repeat([array[-1]], length - len(array), axis=0)
+        ])
+
+
+def resize_with_interpolation(nparray: np.ndarray, length: int) -> np.ndarray:
+    if not isinstance(nparray, np.ndarray):
+        nparray = np.array(nparray)
+    if len(nparray) == length:
+        return nparray
+    if length == 0:
+        return np.zeros((0, *nparray.shape[1:]))
+    cont_indices = np.linspace(0, len(nparray) - 1, length)
+    lh_s = cont_indices.astype(int)
+    rh_s = np.ceil(cont_indices).astype(int)
+    a_s = cont_indices % 1
+    a_s = np.expand_dims(a_s, axis=tuple(range(1, nparray.ndim)))
+    return (1 - a_s) * nparray[lh_s] + a_s * nparray[rh_s]
+
+
+def make_even(
+    iterable_1: Sequence[T],
+    iterable_2: Sequence[S]
+) -> tuple[list[T], list[S]]:
+    len1 = len(iterable_1)
+    len2 = len(iterable_2)
+    if len1 == len2:
+        return iterable_1, iterable_2
+    new_len = max(len1, len2)
+    return (
+        [iterable_1[(n * len1) // new_len] for n in range(new_len)],
+        [iterable_2[(n * len2) // new_len] for n in range(new_len)]
+    )
+
+
+def hash_obj(obj: object) -> int:
+    if isinstance(obj, dict):
+        new_obj = {k: hash_obj(v) for k, v in obj.items()}
+        return hash(tuple(frozenset(sorted(new_obj.items()))))
+
+    if isinstance(obj, (set, tuple, list)):
+        return hash(tuple(hash_obj(e) for e in obj))
+
+    return hash(obj)
```

### Comparing `janim-1.0.4/janim/utils/paths.py` & `janim-1.1.0/janim/utils/paths.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import math
-from typing import Callable
-
-import numpy as np
-
-from janim.constants import OUT
-from janim.utils.bezier import interpolate
-from janim.utils.space_ops import get_norm
-from janim.utils.space_ops import rotation_matrix_transpose
-
-STRAIGHT_PATH_THRESHOLD = 0.01
-
-type PathFunc = Callable[[np.ndarray, np.ndarray, float], np.ndarray]
-
-
-def straight_path(
-    start_points: np.ndarray,
-    end_points: np.ndarray,
-    alpha: float
-) -> np.ndarray:
-    """
-    Same function as interpolate, but renamed to reflect
-    intent of being used to determine how a set of points move
-    to another set.  For instance, it should be a specific case
-    of path_along_arc
-    """
-    return interpolate(start_points, end_points, alpha)
-
-
-def path_along_arc(
-    arc_angle: float,
-    axis: np.ndarray = OUT
-) -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
-    """
-    If vect is vector from start to end, [vect[:,1], -vect[:,0]] is
-    perpendicular to vect in the left direction.
-    """
-    if abs(arc_angle) < STRAIGHT_PATH_THRESHOLD:
-        return straight_path
-    if get_norm(axis) == 0:
-        axis = OUT
-    unit_axis = axis / get_norm(axis)
-
-    def path(start_points, end_points, alpha):
-        vects = end_points - start_points
-        centers = start_points + 0.5 * vects
-        if arc_angle != np.pi:
-            centers += np.cross(unit_axis, vects / 2.0) / math.tan(arc_angle / 2)
-        rot_matrix_T = rotation_matrix_transpose(alpha * arc_angle, unit_axis)
-        return centers + np.dot(start_points - centers, rot_matrix_T)
-
-    return path
-
-
-def clockwise_path() -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
-    return path_along_arc(-np.pi)
-
-
-def counterclockwise_path() -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
-    return path_along_arc(np.pi)
+import math
+from typing import Callable
+
+import numpy as np
+
+from janim.constants import OUT
+from janim.utils.bezier import interpolate
+from janim.utils.space_ops import get_norm
+from janim.utils.space_ops import rotation_matrix_transpose
+
+STRAIGHT_PATH_THRESHOLD = 0.01
+
+type PathFunc = Callable[[np.ndarray, np.ndarray, float], np.ndarray]
+
+
+def straight_path(
+    start_points: np.ndarray,
+    end_points: np.ndarray,
+    alpha: float
+) -> np.ndarray:
+    """
+    Same function as interpolate, but renamed to reflect
+    intent of being used to determine how a set of points move
+    to another set.  For instance, it should be a specific case
+    of path_along_arc
+    """
+    return interpolate(start_points, end_points, alpha)
+
+
+def path_along_arc(
+    arc_angle: float,
+    axis: np.ndarray = OUT
+) -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
+    """
+    If vect is vector from start to end, [vect[:,1], -vect[:,0]] is
+    perpendicular to vect in the left direction.
+    """
+    if abs(arc_angle) < STRAIGHT_PATH_THRESHOLD:
+        return straight_path
+    if get_norm(axis) == 0:
+        axis = OUT
+    unit_axis = axis / get_norm(axis)
+
+    def path(start_points, end_points, alpha):
+        vects = end_points - start_points
+        centers = start_points + 0.5 * vects
+        if arc_angle != np.pi:
+            centers += np.cross(unit_axis, vects / 2.0) / math.tan(arc_angle / 2)
+        rot_matrix_T = rotation_matrix_transpose(alpha * arc_angle, unit_axis)
+        return centers + np.dot(start_points - centers, rot_matrix_T)
+
+    return path
+
+
+def clockwise_path() -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
+    return path_along_arc(-np.pi)
+
+
+def counterclockwise_path() -> Callable[[np.ndarray, np.ndarray, float], np.ndarray]:
+    return path_along_arc(np.pi)
```

### Comparing `janim-1.0.4/janim/utils/rate_functions.py` & `janim-1.1.0/janim/utils/rate_functions.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from typing import Callable
-
-import numpy as np
-
-from janim.utils.bezier import bezier
-
-type RateFunc = Callable[[float], float]
-
-
-def linear(t: float) -> float:
-    return t
-
-
-def smooth(t: float) -> float:
-    # Zero first and second derivatives at t=0 and t=1.
-    # Equivalent to bezier([0, 0, 0, 1, 1, 1])
-    s = 1 - t
-    return (t**3) * (10 * s * s + 5 * s * t + t * t)
-
-
-def rush_into(t: float) -> float:
-    return 2 * smooth(0.5 * t)
-
-
-def rush_from(t: float) -> float:
-    return 2 * smooth(0.5 * (t + 1)) - 1
-
-
-def slow_into(t: float) -> float:
-    return np.sqrt(1 - (1 - t) * (1 - t))
-
-
-def double_smooth(t: float) -> float:
-    if t < 0.5:
-        return 0.5 * smooth(2 * t)
-    else:
-        return 0.5 * (1 + smooth(2 * t - 1))
-
-
-def there_and_back(t: float) -> float:
-    new_t = 2 * t if t < 0.5 else 2 * (1 - t)
-    return smooth(new_t)
-
-
-def there_and_back_with_pause(t: float, pause_ratio: float = 1. / 3) -> float:
-    a = 2. / (1. - pause_ratio)
-    if t < 0.5 - pause_ratio / 2:
-        return smooth(a * t)
-    elif t < 0.5 + pause_ratio / 2:
-        return 1
-    else:
-        return smooth(a - a * t)
-
-
-def running_start(t: float, pull_factor: float = -0.5) -> float:
-    return bezier([0, 0, pull_factor, pull_factor, 1, 1, 1])(t)
-
-
-def not_quite_there(
-    func: RateFunc = smooth,
-    proportion: float = 0.7
-) -> RateFunc:
-    def result(t):
-        return proportion * func(t)
-    return result
-
-
-def wiggle(t: float, wiggles: float = 2) -> float:
-    return there_and_back(t) * np.sin(wiggles * np.pi * t)
-
-
-def squish_rate_func(
-    func: RateFunc,
-    a: float = 0.4,
-    b: float = 0.6
-) -> RateFunc:
-    def result(t):
-        if a == b:
-            return a
-        elif t < a:
-            return func(0)
-        elif t > b:
-            return func(1)
-        else:
-            return func((t - a) / (b - a))
-
-    return result
-
-
-def outside_linear_rate_func(func: RateFunc) -> RateFunc:
-    def result(t):
-        if 0 <= t <= 1:
-            return func(t)
-        return t
-
-    return result
-
-# Stylistically, should this take parameters (with default values)?
-# Ultimately, the functionality is entirely subsumed by squish_rate_func,
-# but it may be useful to have a nice name for with nice default params for
-# "lingering", different from squish_rate_func's default params
-
-
-def lingering(t: float) -> float:
-    return squish_rate_func(lambda t: t, 0, 0.8)(t)
-
-
-def exponential_decay(t: float, half_life: float = 0.1) -> float:
-    # The half-life should be rather small to minimize
-    # the cut-off error at the end
-    return 1 - np.exp(-t / half_life)
+from typing import Callable
+
+import numpy as np
+
+from janim.utils.bezier import bezier
+
+type RateFunc = Callable[[float], float]
+
+
+def linear(t: float) -> float:
+    return t
+
+
+def smooth(t: float) -> float:
+    # Zero first and second derivatives at t=0 and t=1.
+    # Equivalent to bezier([0, 0, 0, 1, 1, 1])
+    s = 1 - t
+    return (t**3) * (10 * s * s + 5 * s * t + t * t)
+
+
+def rush_into(t: float) -> float:
+    return 2 * smooth(0.5 * t)
+
+
+def rush_from(t: float) -> float:
+    return 2 * smooth(0.5 * (t + 1)) - 1
+
+
+def slow_into(t: float) -> float:
+    return np.sqrt(1 - (1 - t) * (1 - t))
+
+
+def double_smooth(t: float) -> float:
+    if t < 0.5:
+        return 0.5 * smooth(2 * t)
+    else:
+        return 0.5 * (1 + smooth(2 * t - 1))
+
+
+def there_and_back(t: float) -> float:
+    new_t = 2 * t if t < 0.5 else 2 * (1 - t)
+    return smooth(new_t)
+
+
+def there_and_back_with_pause(t: float, pause_ratio: float = 1. / 3) -> float:
+    a = 2. / (1. - pause_ratio)
+    if t < 0.5 - pause_ratio / 2:
+        return smooth(a * t)
+    elif t < 0.5 + pause_ratio / 2:
+        return 1
+    else:
+        return smooth(a - a * t)
+
+
+def running_start(t: float, pull_factor: float = -0.5) -> float:
+    return bezier([0, 0, pull_factor, pull_factor, 1, 1, 1])(t)
+
+
+def not_quite_there(
+    func: RateFunc = smooth,
+    proportion: float = 0.7
+) -> RateFunc:
+    def result(t):
+        return proportion * func(t)
+    return result
+
+
+def wiggle(t: float, wiggles: float = 2) -> float:
+    return there_and_back(t) * np.sin(wiggles * np.pi * t)
+
+
+def squish_rate_func(
+    func: RateFunc,
+    a: float = 0.4,
+    b: float = 0.6
+) -> RateFunc:
+    def result(t):
+        if a == b:
+            return a
+        elif t < a:
+            return func(0)
+        elif t > b:
+            return func(1)
+        else:
+            return func((t - a) / (b - a))
+
+    return result
+
+
+def outside_linear_rate_func(func: RateFunc) -> RateFunc:
+    def result(t):
+        if 0 <= t <= 1:
+            return func(t)
+        return t
+
+    return result
+
+# Stylistically, should this take parameters (with default values)?
+# Ultimately, the functionality is entirely subsumed by squish_rate_func,
+# but it may be useful to have a nice name for with nice default params for
+# "lingering", different from squish_rate_func's default params
+
+
+def lingering(t: float) -> float:
+    return squish_rate_func(lambda t: t, 0, 0.8)(t)
+
+
+def exponential_decay(t: float, half_life: float = 0.1) -> float:
+    # The half-life should be rather small to minimize
+    # the cut-off error at the end
+    return 1 - np.exp(-t / half_life)
```

### Comparing `janim-1.0.4/janim/utils/signal.py` & `janim-1.1.0/janim/utils/signal.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-import functools
-import inspect
-from collections import defaultdict
-from dataclasses import dataclass
-from typing import (Callable, Concatenate, Generic, ParamSpec, Self,
-                    TypeVar, overload)
-
-import janim.utils.refresh as refresh
-
-type Key = str
-type FullQualname = str
-
-# 使 sphinx 可用
-P = ParamSpec('P')
-T = TypeVar('T')
-R = TypeVar('R')
-
-
-class _SelfSlots:
-    def __init__(self):
-        self.self_normal_slots: list[Callable] = []
-        self.self_refresh_slots: list[Callable] = []
-        self.self_refresh_slots_with_recurse: list[_SelfSlotWithRecurse] = []
-
-
-class _Slots:
-    def __init__(self):
-        self.normal_slots: list[Callable] = []
-        self.refresh_slots: list[_RefreshSlot] = []
-
-
-class _AllSlots:
-    def __init__(self):
-        self.self_slots_dict: defaultdict[FullQualname, _SelfSlots] = defaultdict(_SelfSlots)
-        self.slots_dict: defaultdict[int, _Slots] = defaultdict(_Slots)
-
-
-@dataclass
-class _SelfSlotWithRecurse:
-    func: Callable
-    recurse_up: bool
-    recurse_down: bool
-
-
-@dataclass
-class _RefreshSlot:
-    obj: refresh.Refreshable
-    func: Callable | str
-
-
-class Signal(Generic[T, P, R]):
-    '''
-    一般用于在 ``func`` 造成影响后，需要对其它数据进行更新时进行作用
-
-    =====
-
-    当 ``func`` 被该类修饰，使用 ``Class.func.emit(self)`` 后，
-
-    对于 ``self_`` 型（修饰）：
-
-    - 会以自身调用所有被 ``func.self_slot()`` 修饰的方法
-    - 会将所有被 ``func.self_refresh()`` 修饰的方法标记需要重新计算
-    - ``func.self_refresh_with_recurse()`` 与 ``func.self_refresh()`` 相比，还可以传入 ``recurse_up/down``
-
-    对于 普通型（绑定）：
-
-    - 会调用所有通过 ``func.connect(...)`` 记录的方法
-    - 会将所有被 ``func.connect_refresh(...)`` 记录的方法标记需要重新计算
-
-    提醒：
-
-    - 可以在上述方法中传入 ``key`` 参数以区分调用
-    - ``emit`` 方法可以传入额外的参数给被调用的 ``slots``
-
-    注意：
-
-    - 以 ``self_`` 开头的修饰器所修饰的方法需要与 ``func`` 在同一个类或者其子类中
-    - ``Signal`` 的绑定与触发相关的调用需要从类名 ``Cls.func.xxx`` 访问，因为 ``obj.func.xxx`` 得到的是原方法
-
-    =====
-
-    例:
-
-    .. code-block:: python
-
-        class User(refresh.Refreshable):
-            def __init__(self, name: str):
-                super().__init__()
-                self.name = name
-                self.msg = ''
-
-            @Signal
-            def set_msg(self, msg: str) -> None:
-                self.msg = msg
-                User.set_msg.emit(self)
-
-            @set_msg.self_slot()
-            def notifier(self) -> None:
-                print("User's message changed")
-
-            @set_msg.self_refresh()
-            @refresh.register
-            def get_text(self) -> str:
-                return f'[{self.name}] {self.msg}'
-
-        user = User('jkjkil')
-        user.set_msg('hello')   # Output: User's message changed
-        print(user.get_text())  # Output: [jkjkil] hello
-
-
-    .. code-block:: python
-
-        class A:
-            @Signal
-            def fn_A(self) -> None:
-                print('fn_A()')
-                A.fn_A.emit(self)
-
-        class B:
-            def fn_B(self) -> None:
-                print('fn_B()')
-
-        a, b = A(), B()
-        A.fn_A.connect(a, b.fn_B)
-
-        a.fn_A()
-        \'\'\'
-        Output:
-        fn_A()
-        fn_B()
-        \'\'\'
-
-
-    另见:
-
-    - :meth:`~.Relation.parents_changed()`
-    - :meth:`~.Relation.children_changed()`
-    '''
-    def __init__(self, func: Callable[Concatenate[T, P], R]):
-        self.func = func
-        functools.update_wrapper(self, func)
-
-        self.slots: defaultdict[Key, _AllSlots] = defaultdict(_AllSlots)
-
-    @overload
-    def __get__(self, instance: None, owner) -> Self: ...
-    @overload
-    def __get__(self, instnace: object, owner) -> Callable[P, R]: ...
-
-    def __get__(self, instance, owner):
-        return self if instance is None else self.func.__get__(instance, owner)
-
-    def __call__(self, *args, **kwargs):    # pragma: no cover
-        return self.func(*args, **kwargs)
-
-    @staticmethod
-    def _get_cls_full_qualname_from_fback() -> str:
-        cls_locals = inspect.currentframe().f_back.f_back.f_locals
-        module = cls_locals['__module__']
-        qualname = cls_locals['__qualname__']
-        return f'{module}.{qualname}'
-
-    @staticmethod
-    def _get_cls_full_qualname(cls: type) -> str:
-        return f'{cls.__module__}.{cls.__qualname__}'
-
-    def self_slot(self, *, key: str = ''):
-        '''
-        被修饰的方法会在 ``Signal`` 触发时被调用
-        '''
-        def decorator(func):
-            full_qualname = self._get_cls_full_qualname_from_fback()
-
-            all_slots = self.slots[key]
-            self_slots = all_slots.self_slots_dict[full_qualname]
-            self_slots.self_normal_slots.append(func)
-
-            return func
-
-        return decorator
-
-    def self_refresh(self, *, key: str = ''):
-        '''
-        被修饰的方法会在 ``Signal`` 触发时，标记需要重新计算
-        '''
-        def decorator(func):
-            full_qualname = self._get_cls_full_qualname_from_fback()
-
-            all_slots = self.slots[key]
-            self_slots = all_slots.self_slots_dict[full_qualname]
-            self_slots.self_refresh_slots.append(func)
-
-            return func
-
-        return decorator
-
-    def self_refresh_with_recurse(self, *, recurse_up: bool = False, recurse_down: bool = False, key: str = ''):
-        '''
-        被修饰的方法会在 ``Signal`` 触发时，标记需要重新计算
-        '''
-        def decorator(func):
-            full_qualname = self._get_cls_full_qualname_from_fback()
-            slot = _SelfSlotWithRecurse(func, recurse_up, recurse_down)
-
-            all_slots = self.slots[key]
-            self_slots = all_slots.self_slots_dict[full_qualname]
-            self_slots.self_refresh_slots_with_recurse.append(slot)
-
-            return func
-
-        return decorator
-
-    def connect(self, sender: object, func: Callable, *, key: str = '') -> None:
-        '''
-        使 ``func`` 会在 ``Signal`` 触发时被调用
-        '''
-        all_slots = self.slots[key]
-        slots = all_slots.slots_dict[id(sender)]
-        slots.normal_slots.append(func)
-
-    def connect_refresh(self, sender: object, obj: object, func: Callable | str, *, key: str = '') -> None:
-        '''
-        使 ``func`` 会在 ``Signal`` 触发时被标记为需要重新计算
-        '''
-        slot = _RefreshSlot(obj, func)
-
-        all_slots = self.slots[key]
-        slots = all_slots.slots_dict[id(sender)]
-        slots.refresh_slots.append(slot)
-
-    def emit(self, sender: object, *args, key: str = '', **kwargs):
-        '''
-        触发 ``Signal``
-        '''
-        all_slots = self.slots.get(key, None)
-        if all_slots is None:
-            return
-
-        for cls in sender.__class__.mro():
-            full_qualname = self._get_cls_full_qualname(cls)
-            if full_qualname not in all_slots.self_slots_dict:
-                continue
-
-            slots = all_slots.self_slots_dict[full_qualname]
-
-            # self_normal_slots
-            for func in slots.self_normal_slots:
-                func(sender, *args, **kwargs)
-
-            # self_refresh_slots
-            for func in slots.self_refresh_slots:
-                sender.mark_refresh(func)
-
-            # self_refresh_slots_with_recurse
-            for slot in slots.self_refresh_slots_with_recurse:
-                sender.mark_refresh(slot.func, recurse_up=slot.recurse_up, recurse_down=slot.recurse_down)
-
-        sender_id = id(sender)
-        if sender_id in all_slots.slots_dict:
-            slots = all_slots.slots_dict[sender_id]
-
-            # normal_slots
-            for func in slots.normal_slots:
-                func(*args, **kwargs)
-
-            # refresh_slots
-            for slot in slots.refresh_slots:
-                slot.obj.mark_refresh(slot.func)
+import functools
+import inspect
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import (Callable, Concatenate, Generic, ParamSpec, Self,
+                    TypeVar, overload)
+
+import janim.utils.refresh as refresh
+
+type Key = str
+type FullQualname = str
+
+# 使 sphinx 可用
+P = ParamSpec('P')
+T = TypeVar('T')
+R = TypeVar('R')
+
+
+class _SelfSlots:
+    def __init__(self):
+        self.self_normal_slots: list[Callable] = []
+        self.self_refresh_slots: list[Callable] = []
+        self.self_refresh_slots_with_recurse: list[_SelfSlotWithRecurse] = []
+
+
+class _Slots:
+    def __init__(self):
+        self.normal_slots: list[Callable] = []
+        self.refresh_slots: list[_RefreshSlot] = []
+
+
+class _AllSlots:
+    def __init__(self):
+        self.self_slots_dict: defaultdict[FullQualname, _SelfSlots] = defaultdict(_SelfSlots)
+        self.slots_dict: defaultdict[int, _Slots] = defaultdict(_Slots)
+
+
+@dataclass
+class _SelfSlotWithRecurse:
+    func: Callable
+    recurse_up: bool
+    recurse_down: bool
+
+
+@dataclass
+class _RefreshSlot:
+    obj: refresh.Refreshable
+    func: Callable | str
+
+
+class Signal(Generic[T, P, R]):
+    '''
+    一般用于在 ``func`` 造成影响后，需要对其它数据进行更新时进行作用
+
+    =====
+
+    当 ``func`` 被该类修饰，使用 ``Class.func.emit(self)`` 后，
+
+    对于 ``self_`` 型（修饰）：
+
+    - 会以自身调用所有被 ``func.self_slot()`` 修饰的方法
+    - 会将所有被 ``func.self_refresh()`` 修饰的方法标记需要重新计算
+    - ``func.self_refresh_with_recurse()`` 与 ``func.self_refresh()`` 相比，还可以传入 ``recurse_up/down``
+
+    对于 普通型（绑定）：
+
+    - 会调用所有通过 ``func.connect(...)`` 记录的方法
+    - 会将所有被 ``func.connect_refresh(...)`` 记录的方法标记需要重新计算
+
+    提醒：
+
+    - 可以在上述方法中传入 ``key`` 参数以区分调用
+    - ``emit`` 方法可以传入额外的参数给被调用的 ``slots``
+
+    注意：
+
+    - 以 ``self_`` 开头的修饰器所修饰的方法需要与 ``func`` 在同一个类或者其子类中
+    - ``Signal`` 的绑定与触发相关的调用需要从类名 ``Cls.func.xxx`` 访问，因为 ``obj.func.xxx`` 得到的是原方法
+
+    =====
+
+    例:
+
+    .. code-block:: python
+
+        class User(refresh.Refreshable):
+            def __init__(self, name: str):
+                super().__init__()
+                self.name = name
+                self.msg = ''
+
+            @Signal
+            def set_msg(self, msg: str) -> None:
+                self.msg = msg
+                User.set_msg.emit(self)
+
+            @set_msg.self_slot()
+            def notifier(self) -> None:
+                print("User's message changed")
+
+            @set_msg.self_refresh()
+            @refresh.register
+            def get_text(self) -> str:
+                return f'[{self.name}] {self.msg}'
+
+        user = User('jkjkil')
+        user.set_msg('hello')   # Output: User's message changed
+        print(user.get_text())  # Output: [jkjkil] hello
+
+
+    .. code-block:: python
+
+        class A:
+            @Signal
+            def fn_A(self) -> None:
+                print('fn_A()')
+                A.fn_A.emit(self)
+
+        class B:
+            def fn_B(self) -> None:
+                print('fn_B()')
+
+        a, b = A(), B()
+        A.fn_A.connect(a, b.fn_B)
+
+        a.fn_A()
+        \'\'\'
+        Output:
+        fn_A()
+        fn_B()
+        \'\'\'
+
+
+    另见:
+
+    - :meth:`~.Relation.parents_changed()`
+    - :meth:`~.Relation.children_changed()`
+    '''
+    def __init__(self, func: Callable[Concatenate[T, P], R]):
+        self.func = func
+        functools.update_wrapper(self, func)
+
+        self.slots: defaultdict[Key, _AllSlots] = defaultdict(_AllSlots)
+
+    @overload
+    def __get__(self, instance: None, owner) -> Self: ...
+    @overload
+    def __get__(self, instnace: object, owner) -> Callable[P, R]: ...
+
+    def __get__(self, instance, owner):
+        return self if instance is None else self.func.__get__(instance, owner)
+
+    def __call__(self, *args, **kwargs):    # pragma: no cover
+        return self.func(*args, **kwargs)
+
+    @staticmethod
+    def _get_cls_full_qualname_from_fback() -> str:
+        cls_locals = inspect.currentframe().f_back.f_back.f_locals
+        module = cls_locals['__module__']
+        qualname = cls_locals['__qualname__']
+        return f'{module}.{qualname}'
+
+    @staticmethod
+    def _get_cls_full_qualname(cls: type) -> str:
+        return f'{cls.__module__}.{cls.__qualname__}'
+
+    def self_slot(self, *, key: str = ''):
+        '''
+        被修饰的方法会在 ``Signal`` 触发时被调用
+        '''
+        def decorator(func):
+            full_qualname = self._get_cls_full_qualname_from_fback()
+
+            all_slots = self.slots[key]
+            self_slots = all_slots.self_slots_dict[full_qualname]
+            self_slots.self_normal_slots.append(func)
+
+            return func
+
+        return decorator
+
+    def self_refresh(self, *, key: str = ''):
+        '''
+        被修饰的方法会在 ``Signal`` 触发时，标记需要重新计算
+        '''
+        def decorator(func):
+            full_qualname = self._get_cls_full_qualname_from_fback()
+
+            all_slots = self.slots[key]
+            self_slots = all_slots.self_slots_dict[full_qualname]
+            self_slots.self_refresh_slots.append(func)
+
+            return func
+
+        return decorator
+
+    def self_refresh_with_recurse(self, *, recurse_up: bool = False, recurse_down: bool = False, key: str = ''):
+        '''
+        被修饰的方法会在 ``Signal`` 触发时，标记需要重新计算
+        '''
+        def decorator(func):
+            full_qualname = self._get_cls_full_qualname_from_fback()
+            slot = _SelfSlotWithRecurse(func, recurse_up, recurse_down)
+
+            all_slots = self.slots[key]
+            self_slots = all_slots.self_slots_dict[full_qualname]
+            self_slots.self_refresh_slots_with_recurse.append(slot)
+
+            return func
+
+        return decorator
+
+    def connect(self, sender: object, func: Callable, *, key: str = '') -> None:
+        '''
+        使 ``func`` 会在 ``Signal`` 触发时被调用
+        '''
+        all_slots = self.slots[key]
+        slots = all_slots.slots_dict[id(sender)]
+        slots.normal_slots.append(func)
+
+    def connect_refresh(self, sender: object, obj: object, func: Callable | str, *, key: str = '') -> None:
+        '''
+        使 ``func`` 会在 ``Signal`` 触发时被标记为需要重新计算
+        '''
+        slot = _RefreshSlot(obj, func)
+
+        all_slots = self.slots[key]
+        slots = all_slots.slots_dict[id(sender)]
+        slots.refresh_slots.append(slot)
+
+    def emit(self, sender: object, *args, key: str = '', **kwargs):
+        '''
+        触发 ``Signal``
+        '''
+        all_slots = self.slots.get(key, None)
+        if all_slots is None:
+            return
+
+        for cls in sender.__class__.mro():
+            full_qualname = self._get_cls_full_qualname(cls)
+            if full_qualname not in all_slots.self_slots_dict:
+                continue
+
+            slots = all_slots.self_slots_dict[full_qualname]
+
+            # self_normal_slots
+            for func in slots.self_normal_slots:
+                func(sender, *args, **kwargs)
+
+            # self_refresh_slots
+            for func in slots.self_refresh_slots:
+                sender.mark_refresh(func)
+
+            # self_refresh_slots_with_recurse
+            for slot in slots.self_refresh_slots_with_recurse:
+                sender.mark_refresh(slot.func, recurse_up=slot.recurse_up, recurse_down=slot.recurse_down)
+
+        sender_id = id(sender)
+        if sender_id in all_slots.slots_dict:
+            slots = all_slots.slots_dict[sender_id]
+
+            # normal_slots
+            for func in slots.normal_slots:
+                func(*args, **kwargs)
+
+            # refresh_slots
+            for slot in slots.refresh_slots:
+                slot.obj.mark_refresh(slot.func)
```

### Comparing `janim-1.0.4/logo.png` & `janim-1.1.0/logo.png`

 * *Files identical despite different names*

### Comparing `janim-1.0.4/PKG-INFO` & `janim-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a61 6e69  : 2.1.Name: jani
-00000020: 6d0a 5665 7273 696f 6e3a 2031 2e30 2e34  m.Version: 1.0.4
+00000020: 6d0a 5665 7273 696f 6e3a 2031 2e31 2e30  m.Version: 1.1.0
 00000030: 0a53 756d 6d61 7279 3a20 6120 6c69 6272  .Summary: a libr
 00000040: 6172 7920 666f 7220 7369 6d70 6c65 2061  ary for simple a
 00000050: 6e69 6d61 7469 6f6e 2065 6666 6563 7473  nimation effects
 00000060: 0a41 7574 686f 723a 206a 6b6a 6b69 6c34  .Author: jkjkil4
 00000070: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 00000080: 3a20 3e3d 332e 3132 0a44 6573 6372 6970  : >=3.12.Descrip
 00000090: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
@@ -77,49 +77,64 @@
 000004c0: 496e 7472 6f64 7563 7469 6f6e 0a4a 416e  Introduction.JAn
 000004d0: 696d 2069 7320 6120 6c69 6272 6172 7920  im is a library 
 000004e0: 666f 7220 7369 6d70 6c65 2061 6e69 6d61  for simple anima
 000004f0: 7469 6f6e 2065 6666 6563 7473 2e0a 0a49  tion effects...I
 00000500: 6e73 7069 7265 6420 6279 205b 6d61 6e69  nspired by [mani
 00000510: 6d5d 2868 7474 7073 3a2f 2f67 6974 6875  m](https://githu
 00000520: 622e 636f 6d2f 3362 3162 2f6d 616e 696d  b.com/3b1b/manim
-00000530: 292e 0a0a 0a23 2320 496e 7374 616c 6c61  )....## Installa
-00000540: 7469 6f6e 0a4a 416e 696d 2072 756e 7320  tion.JAnim runs 
-00000550: 6f6e 2050 7974 686f 6e20 332e 3132 2b20  on Python 3.12+ 
-00000560: 616e 6420 4f70 656e 474c 2034 2e33 2b2e  and OpenGL 4.3+.
-00000570: 0a0a 596f 7520 6d61 7920 696e 7374 616c  ..You may instal
-00000580: 6c20 4a41 6e69 6d20 6469 7265 6374 6c79  l JAnim directly
-00000590: 2076 6961 0a60 6060 7368 0a70 6970 2069   via.```sh.pip i
-000005a0: 6e73 7461 6c6c 206a 616e 696d 0a60 6060  nstall janim.```
-000005b0: 0a74 6f20 696e 7374 616c 6c20 7468 6520  .to install the 
-000005c0: 6c61 7465 7374 2076 6572 7369 6f6e 2064  latest version d
-000005d0: 6973 7472 6962 7574 6564 206f 6e20 7079  istributed on py
-000005e0: 7069 2e20 4f72 2c20 746f 2063 6174 6368  pi. Or, to catch
-000005f0: 2075 7020 7769 7468 2074 6865 206c 6174   up with the lat
-00000600: 6573 7420 6465 7665 6c6f 706d 656e 7420  est development 
-00000610: 616e 6420 6564 6974 2074 6865 2073 6f75  and edit the sou
-00000620: 7263 6520 636f 6465 2c20 796f 7520 6d61  rce code, you ma
-00000630: 7920 636c 6f6e 6520 7468 6973 2072 6570  y clone this rep
-00000640: 6f73 6974 6f72 7920 7669 610a 6060 6073  ository via.```s
-00000650: 680a 6769 7420 636c 6f6e 6520 6874 7470  h.git clone http
-00000660: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00000670: 6b6a 6b69 6c34 2f4a 416e 696d 2e67 6974  kjkil4/JAnim.git
-00000680: 0a63 6420 4a41 6e69 6d0a 7069 7020 696e  .cd JAnim.pip in
-00000690: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
-000006a0: 4164 6469 7469 6f6e 616c 6c79 2c20 7468  Additionally, th
-000006b0: 6572 6520 6172 6520 6f74 6865 7220 736f  ere are other so
-000006c0: 6674 7761 7265 2064 6570 656e 6465 6e63  ftware dependenc
-000006d0: 6965 7320 746f 2062 6520 696e 7374 616c  ies to be instal
-000006e0: 6c65 643a 0a2d 2054 6f20 6765 6e65 7261  led:.- To genera
-000006f0: 7465 2076 6964 656f 2066 696c 6573 2c20  te video files, 
-00000700: 696e 7374 616c 6c20 5b66 666d 7065 675d  install [ffmpeg]
-00000710: 2868 7474 7073 3a2f 2f66 666d 7065 672e  (https://ffmpeg.
-00000720: 6f72 672f 292e 0a2d 2054 6f20 7573 6520  org/)..- To use 
-00000730: 6054 7970 7374 602c 2069 6e73 7461 6c6c  `Typst`, install
-00000740: 205b 7479 7073 745d 2868 7474 7073 3a2f   [typst](https:/
-00000750: 2f67 6974 6875 622e 636f 6d2f 7479 7073  /github.com/typs
-00000760: 742f 7479 7073 7429 2e0a 0a0a 2323 2055  t/typst)....## U
-00000770: 7369 6e67 204a 416e 696d 0a0a 596f 7520  sing JAnim..You 
-00000780: 6361 6e20 7275 6e0a 6060 6073 680a 6a61  can run.```sh.ja
-00000790: 6e69 6d20 6578 616d 706c 6573 0a60 6060  nim examples.```
-000007a0: 0a74 6f20 7365 6520 6578 616d 706c 6573  .to see examples
-000007b0: 2e0a 0a0a 2323 204c 6963 656e 7365 0a0a  ....## License..
-000007c0: 4d49 5420 6c69 6365 6e73 650a 0a         MIT license..
+00000530: 292e 0a0a 3c74 6162 6c65 3e0a 2020 3c74  )...<table>.  <t
+00000540: 723e 0a20 2020 203c 7464 3e0a 2020 2020  r>.    <td>.    
+00000550: 2020 3c69 6d67 2073 7263 3d22 2e2f 6173    <img src="./as
+00000560: 7365 7473 2f57 7269 7465 4578 616d 706c  sets/WriteExampl
+00000570: 652e 6769 6622 2f3e 0a20 2020 203c 2f74  e.gif"/>.    </t
+00000580: 643e 0a20 2020 203c 7464 3e0a 2020 2020  d>.    <td>.    
+00000590: 2020 3c69 6d67 2073 7263 3d22 2e2f 6173    <img src="./as
+000005a0: 7365 7473 2f54 6578 7445 7861 6d70 6c65  sets/TextExample
+000005b0: 2e67 6966 222f 3e0a 2020 2020 3c2f 7464  .gif"/>.    </td
+000005c0: 3e0a 2020 2020 3c74 643e 0a20 2020 2020  >.    <td>.     
+000005d0: 203c 696d 6720 7372 633d 222e 2f61 7373   <img src="./ass
+000005e0: 6574 732f 4e75 6d62 6572 506c 616e 6545  ets/NumberPlaneE
+000005f0: 7861 6d70 6c65 2e67 6966 222f 3e0a 2020  xample.gif"/>.  
+00000600: 2020 3c2f 7464 3e0a 2020 3c2f 7472 3e0a    </td>.  </tr>.
+00000610: 3c2f 7461 626c 653e 0a0a 2323 2049 6e73  </table>..## Ins
+00000620: 7461 6c6c 6174 696f 6e0a 4a41 6e69 6d20  tallation.JAnim 
+00000630: 7275 6e73 206f 6e20 5079 7468 6f6e 2033  runs on Python 3
+00000640: 2e31 322b 2061 6e64 204f 7065 6e47 4c20  .12+ and OpenGL 
+00000650: 342e 332b 2e0a 0a59 6f75 206d 6179 2069  4.3+...You may i
+00000660: 6e73 7461 6c6c 204a 416e 696d 2064 6972  nstall JAnim dir
+00000670: 6563 746c 7920 7669 610a 6060 6073 680a  ectly via.```sh.
+00000680: 7069 7020 696e 7374 616c 6c20 6a61 6e69  pip install jani
+00000690: 6d0a 6060 600a 746f 2069 6e73 7461 6c6c  m.```.to install
+000006a0: 2074 6865 206c 6174 6573 7420 7665 7273   the latest vers
+000006b0: 696f 6e20 6469 7374 7269 6275 7465 6420  ion distributed 
+000006c0: 6f6e 2070 7970 692e 204f 722c 2074 6f20  on pypi. Or, to 
+000006d0: 6361 7463 6820 7570 2077 6974 6820 7468  catch up with th
+000006e0: 6520 6c61 7465 7374 2064 6576 656c 6f70  e latest develop
+000006f0: 6d65 6e74 2061 6e64 2065 6469 7420 7468  ment and edit th
+00000700: 6520 736f 7572 6365 2063 6f64 652c 2079  e source code, y
+00000710: 6f75 206d 6179 2063 6c6f 6e65 2074 6869  ou may clone thi
+00000720: 7320 7265 706f 7369 746f 7279 2076 6961  s repository via
+00000730: 0a60 6060 7368 0a67 6974 2063 6c6f 6e65  .```sh.git clone
+00000740: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000750: 636f 6d2f 6a6b 6a6b 696c 342f 4a41 6e69  com/jkjkil4/JAni
+00000760: 6d2e 6769 740a 6364 204a 416e 696d 0a70  m.git.cd JAnim.p
+00000770: 6970 2069 6e73 7461 6c6c 202d 6520 2e0a  ip install -e ..
+00000780: 6060 600a 0a41 6464 6974 696f 6e61 6c6c  ```..Additionall
+00000790: 792c 2074 6865 7265 2061 7265 206f 7468  y, there are oth
+000007a0: 6572 2073 6f66 7477 6172 6520 6465 7065  er software depe
+000007b0: 6e64 656e 6369 6573 2074 6f20 6265 2069  ndencies to be i
+000007c0: 6e73 7461 6c6c 6564 3a0a 2d20 546f 2067  nstalled:.- To g
+000007d0: 656e 6572 6174 6520 7669 6465 6f20 6669  enerate video fi
+000007e0: 6c65 732c 2069 6e73 7461 6c6c 205b 6666  les, install [ff
+000007f0: 6d70 6567 5d28 6874 7470 733a 2f2f 6666  mpeg](https://ff
+00000800: 6d70 6567 2e6f 7267 2f29 2e0a 2d20 546f  mpeg.org/)..- To
+00000810: 2075 7365 2060 5479 7073 7460 2c20 696e   use `Typst`, in
+00000820: 7374 616c 6c20 5b74 7970 7374 5d28 6874  stall [typst](ht
+00000830: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000840: 2f74 7970 7374 2f74 7970 7374 292e 0a0a  /typst/typst)...
+00000850: 0a23 2320 5573 696e 6720 4a41 6e69 6d0a  .## Using JAnim.
+00000860: 0a59 6f75 2063 616e 2072 756e 0a60 6060  .You can run.```
+00000870: 7368 0a6a 616e 696d 2065 7861 6d70 6c65  sh.janim example
+00000880: 730a 6060 600a 746f 2073 6565 2065 7861  s.```.to see exa
+00000890: 6d70 6c65 732e 0a0a 0a23 2320 4c69 6365  mples....## Lice
+000008a0: 6e73 650a 0a4d 4954 206c 6963 656e 7365  nse..MIT license
+000008b0: 0a0a                                     ..
```

